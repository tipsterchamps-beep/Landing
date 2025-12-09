<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8" />
  <title>TipsterChamps App (Demo)</title>
  <meta name="viewport" content="width=device-width, initial-scale=1.0" />
</head>
<body>
  <h1>TipsterChamps – Demo de Picks</h1>

  <form id="pick-form">
    <input type="text" id="username" placeholder="Tu nombre" required />
    <input type="text" id="team" placeholder="Equipo elegido" required />
    <button type="submit">Guardar pick</button>
  </form>

  <h2>Picks guardados</h2>
  <ul id="picks-list"></ul>

  <!-- SDK de Supabase -->
  <script type="module">
    import { createClient } from 'https://esm.sh/@supabase/supabase-js@2';

    const SUPABASE_URL = 'TU_URL_AQUI';
    const SUPABASE_ANON_KEY = 'TU_ANON_KEY_AQUI';

    const supabase = createClient(SUPABASE_URL, SUPABASE_ANON_KEY);

    const form = document.getElementById('pick-form');
    const list = document.getElementById('picks-list');

    async function loadPicks() {
      const { data, error } = await supabase
        .from('picks_demo')
        .select('*')
        .order('created_at', { ascending: false });

      if (error) {
        console.error(error);
        return;
      }

      list.innerHTML = '';
      data.forEach(pick => {
        const li = document.createElement('li');
        li.textContent = `${pick.user_name} → ${pick.team}`;
        list.appendChild(li);
      });
    }

    form.addEventListener('submit', async (e) => {
      e.preventDefault();
      const user_name = document.getElementById('username').value;
      const team = document.getElementById('team').value;

      const { error } = await supabase
        .from('picks_demo')
        .insert([{ user_name, team }]);

      if (error) {
        console.error(error);
        alert('Error guardando pick');
      } else {
        form.reset();
        loadPicks();
      }
    });

    loadPicks();
  </script>
</body>
</html>
