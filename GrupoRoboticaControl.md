---
marp: true
theme: default
paginate: true
html: true
footer: 'Grupo de Robótica y Control · Tecnun – Universidad de Navarra'
backgroundColor: #fff
style: |
  section {
    font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
    position: relative !important;
    display: flex;
    flex-direction: column;
    justify-content: flex-start;
    padding-top: 70px;
    color: #1e293b;
  }
  section::after { color: #94a3b8; font-size: 16px; }
  section footer {
    position: absolute !important;
    bottom: 20px !important; left: 40px !important; right: 40px !important;
    font-size: 14px !important; color: #888 !important;
    border-top: 1px solid #eee !important; padding-top: 10px !important;
  }
  h1 {
    color: #2b5b8c;
    border-left: 8px solid #c8102e;
    padding-left: 20px;
    font-size: 50px;
    margin: 0 0 0.5em 0;
  }
  img.logo-corner {
    position: absolute; top: 28px; right: 40px; height: 60px;
  }

  /* Portada */
  section.cover {
    padding: 0; justify-content: center;
    background: radial-gradient(circle at 45% 100%, #6fa8c8 0%, #2b5b8c 55%, #1d3f63 100%);
  }
  section.cover.red { background: radial-gradient(circle at 45% 100%, #ff2a2a 0%, #e00000 60%, #b80000 100%); }
  section.cover footer, section.cover::after { display: none; }
  .cover-title { position: absolute; top: 50px; left: 80px; width: 420px; }
  .cover-logo { position: absolute; bottom: 45px; left: 95px; width: 200px; }
  .cover-robot { position: absolute; bottom: 0; right: 40px; height: 95%; }
  .cover-robot.small { height: 62%; }

  /* Tarjetas */
  .cards { display: grid; gap: 22px; margin-top: 10px; }
  .cards.c4 { grid-template-columns: repeat(4, 1fr); }
  .cards.c3 { grid-template-columns: repeat(3, 1fr); }
  .card {
    background: #f1f5f9; border-radius: 18px; padding: 22px 24px;
    border-left: 8px solid #2b5b8c; font-size: 22px; line-height: 1.5;
    box-shadow: 0 4px 10px rgba(0,0,0,0.06);
  }
  .card:nth-child(even) { border-left-color: #6fa8c8; }
  .card h3 { margin: 0 0 12px 0; font-size: 26px; color: #0f172a; text-transform: uppercase; }
  .card ul { margin: 0; padding-left: 0; list-style: none; }
  .card img { display: block; margin: 14px auto 0; max-height: 110px; }
  .prio { margin-top: 18px; font-weight: 600; font-size: 20px; }
  .dot { display: inline-block; width: 18px; height: 18px; border-radius: 50%; vertical-align: -2px; margin-right: 8px; }
  .alta { background: #e00000; } .media { background: #f08a00; } .ok { background: #22a845; }

  section.equip .card { font-size: 16px; line-height: 1.35; padding: 16px 18px; }
  section.equip .card h3 { font-size: 21px; margin-bottom: 8px; }
  section.equip .card img { max-height: 70px; margin-top: 8px; }
  .two { display: grid; grid-template-columns: 1.4fr 1fr; gap: 40px; align-items: center; }
  .two img { max-height: 520px; justify-self: center; }
  .lead { font-size: 30px; line-height: 1.6; }

  /* Tablas */
  table { width: 100%; border-collapse: collapse; font-size: 22px; }
  th { background: #2b5b8c; color: #fff; text-align: left; padding: 8px 12px; }
  td { padding: 6px 12px; border-bottom: 1px solid #cbd5e1; vertical-align: middle; }
  tr:nth-child(even) td { background: #f1f5f9; }
  td img.avatar { width: 40px; height: 40px; border-radius: 50%; vertical-align: middle; margin-left: 8px; }
  section.people { padding-top: 45px; }
  section.people h1 { font-size: 40px; margin-bottom: 0.3em; }
  section.people table { font-size: 17px; }
  section.people .growth, section.people .legend { font-size: 17px; }
  section.people td { padding: 3px 12px; }
  section.people td img.avatar { width: 28px; height: 28px; }
  section.projects { padding-top: 50px; }
  section.projects h1 { font-size: 40px; margin-bottom: 0.3em; }
  section.projects table { font-size: 12.5px; line-height: 1.2; }
  section.projects td, section.projects th { padding: 3px 6px; }
  .pend { color: #c8102e; } .act { color: #22a845; font-weight: 600; }
  .legend { font-size: 20px; line-height: 1.6; }
  .growth { font-size: 20px; color: #475569; }
  .tag { color: #c8102e; font-weight: 600; }

  /* Objetivos */
  .goals { display: grid; grid-template-columns: repeat(5, 1fr); gap: 14px; text-align: center; }
  .goal { border: 2px solid #2b5b8c; border-radius: 18px; padding: 26px 12px; font-size: 20px; }
  .goal .ic { font-size: 54px; }
  .goal b { display: block; font-size: 24px; margin: 10px 0; }
  .mission { margin-top: 30px; font-size: 24px; font-weight: 700; color: #1d3f63; text-align: justify; }

  /* Club */
  section.splash { justify-content: center; align-items: center; }
  section.splash img { width: 60%; }
  .club { display: grid; grid-template-columns: 1fr 1fr; gap: 30px; align-items: center; }
  .item { background: #f1f5f9; border-radius: 12px; padding: 14px 18px; margin: 12px 0; font-size: 22px; }
  .robots { display: flex; gap: 10px; align-items: flex-end; justify-content: center; }
  .robots img { height: 190px; }
---

<!-- _class: cover -->
<!-- _backgroundColor: #2b5b8c -->
<!-- _backgroundImage: "radial-gradient(circle at 45% 100%, #6fa8c8 0%, #2b5b8c 55%, #1d3f63 100%)" -->
<img class="cover-title" src="images/title_text.png" alt="Grupo de Robótica y Control" />
<img class="cover-logo" src="images/tecnun_white.png" alt="Tecnun Universidad de Navarra" />
<img class="cover-robot" src="images/humanoide1.png" alt="Robot humanoide" />

---

# Quiénes somos
<img class="logo-corner" src="images/tecnun_red.png" />

<div class="two">
<div class="lead">

Grupo multidisciplinar que investiga y desarrolla soluciones de **robótica**, **automatización** y **sistemas mecatrónicos** para la industria del futuro.

Trabajamos en robótica industrial y colaborativa, robótica móvil y tecnologías hápticas, integrando *control avanzado*, *IA*, *visión artificial*, *realidad aumentada* y *gemelos digitales*.

</div>
<img src="images/ur.png" alt="Robot colaborativo" />
</div>

---

# Visión general del grupo
<img class="logo-corner" src="images/tecnun_red.png" />

<div class="cards c4">
<div class="card"><h3>Personas</h3><ul><li>Investigadores actuales</li><li>Doctorandos actuales</li><li>Incorporaciones previstas</li></ul></div>
<div class="card"><h3>Investigación</h3><ul><li>Robótica y control</li><li>Mecatrónica</li><li>IA y visión artificial</li><li>Tecnologías hápticas</li></ul></div>
<div class="card"><h3>Proyectos</h3><ul><li>En curso</li><li>Propuestas previstas</li><li>Colaboraciones</li></ul></div>
<div class="card"><h3>Infraestructura</h3><ul><li>Robots y manipuladores</li><li>Visión y sensores</li><li>Control y automatización</li><li>Simulación</li></ul></div>
</div>

---

<!-- _class: people -->
# Investigadores y doctorandos
<img class="logo-corner" src="images/tecnun_red.png" />

| Persona | Perfil | Línea / actividad | Situación |
|---|---|---|---|
| Sebastián Gutiérrez <img class="avatar" src="images/sebastian.jpg"> | Investigador/a ♪ | Robótica · Control · IA | Tecnun |
| Jorge Juan Gil <img class="avatar" src="images/jorge.jpg"> | Investigador/a | Robótica · Control · IA | Tecnun |
| Diego Borro Yagüez <img class="avatar" src="images/diego.jpg"> | Investigador/a ↑ | Visión · IA | Tecnun |
| Iñaki Díaz Garmendia <img class="avatar" src="images/inaki.jpg"> | Investigador/a | Robótica · Control | Ceit |
| Emilio Sánchez Tapia <img class="avatar" src="images/emilio.jpg"> | Investigador/a | Robótica | Ceit |
| Wilson Brian Mesa <img class="avatar" src="images/wilson.jpg"> | Doctorando/a ↓ | Robótica · Control | Tecnun |
| Julie Laurent <img class="avatar" src="images/julie.jpg"> | Técnico/a | Robótica | Tecnun |

<div class="two" style="grid-template-columns: 1.3fr 1fr; margin-top: 14px;">
<div class="growth">

**Plan de crecimiento del grupo (2026-2030)**
- 3 nuevas incorporaciones de doctorado <span class="tag">DESEABLE</span>
- 1 perfil estratégico en Robótica e IA (Técnico de Laboratorio) <span class="tag">DESEABLE</span>

</div>
<div class="legend">
<span style="color:#0ea5e9">♪ Responsable del grupo</span><br>
<span style="color:#22a845">↑ Incorporación: ene. 2026</span><br>
<span style="color:#e00000">↓ Finalización prevista: ene. 2027</span>
</div>
</div>

---

# Líneas de investigación
<img class="logo-corner" src="images/tecnun_red.png" />

<div class="two">
<div class="lead" style="font-size: 24px; line-height:1.45;">

- Robótica avanzada (industrial, colaborativa y humanoide)
- Automatización, control y sistemas autónomos
- Mecatrónica y sistemas inteligentes
- Visión artificial e inteligencia artificial aplicada
- Interacción humano-robot y tecnologías hápticas
- Gemelos digitales y simulación industrial
- IoT y sistemas conectados para Industria 4.0

</div>
<img src="images/humanoide2.png" alt="Robot humanoide" />
</div>

---

<!-- _class: projects -->
# Proyectos de investigación 2023 – 2026
<img class="logo-corner" src="images/tecnun_red.png" />

| Nombre | Acrónimo | Rol | Convocatoria | Tipo | Importe | Inicio | Fin | Comentario |
|---|---|---|---|---|---|---|---|---|
| Learning-based Adaptive Robotic Reach with Unified visuo-tactile Architectures | LARRUA | Líder | PIBA 2026 | Regional | 80.000,00 € | | | <span class="pend">Pendiente de resolución</span> |
| Learning-based Adaptive Robotic Reach with Unified visuo-tactile Architectures | LARRUA | Líder | DFG Zientzia 2026 | Regional | 120.709,31 € | | | <span class="pend">Pendiente de resolución</span> |
| Investigación y desarrollo de tecnologías IA para dotar de máxima autonomía a la fabricación y reparación mediante procesos DED de piezas de gran tamaño y de alto valor añadido (FactorIA) | FACTOR(IA) | Part. | AEI - Transmisiones | Nacional | 328.609,50 € | 01/01/2025 | 31/12/2028 | <span class="act">Activo</span> |
| PIUNA | PIUNA | Part. | | UNAV | | | | |
| Investigación de nuevos Modelos Reducidos basados en la física para la Digitalización Industrial (MoReDigital) | MoreDigi | Part. | Elkartek 2024 | Regional | 216.611,00 € | 01/04/2024 | 31/03/2026 | Finalizado |
| Beca Leonardo | | Líder | Becas Leonardo | Nacional | 50.000,00 € | | | Denegado |
| Investigación de nuevos Modelos Reducidos basados en la física, enriquecidos con DATos y Aprendizaje automático | MoreData | Part. | Elkartek 2026 | Regional | 598.165,07 € | | | Denegado |
| Diseño de algoritmos inteligentes para utilización en BESS | SMART BESS | Líder | DFG I+D 2025 | Regional | 94.413,00 € | | | Denegado |
| Métodos y algoritmos para la automatización en la digitalización holística inmersiva de la fábrica (LANVERSO) | LANVERSO | Part. | Elkartek 2022 | Regional | 83.478,00 € | 01/03/2022 | 31/12/2023 | Finalizado |

---

<!-- _class: equip -->
# Equipamiento actual
<img class="logo-corner" src="images/tecnun_red.png" />

<div class="cards c4">
<div class="card"><h3>Robótica</h3><ul><li>Franka Emika Panda</li><li>Franka Research 3 (FR3)</li><li>Stäubli TX60</li><li>Fanuc LR Mate 200iB</li><li>Fanuc M-10iA</li><li>Gripper Robotiq</li><li>Robot cartesiano Aula Biele</li><li>Mitsubishi PA-10 <span class="tag">(Descontinuado)</span></li></ul><img src="images/franka.png"></div>
<div class="card"><h3>Visión</h3><ul><li>Intel RealSense D405</li><li>Sensórica</li></ul><img src="images/realsense.png"><h3 style="margin-top:22px">Háptica</h3><ul><li>Phantom Premium 1.5</li><li>Phantom Premium 1.0</li><li>Phantom Omni ×3</li></ul><img src="images/phantom.png"></div>
<div class="card"><h3>Control</h3><ul><li>PLC Beckhoff</li><li>Jetson Nano</li><li>Arduino R4 Wifi</li><li>Arduino Q</li></ul><img src="images/plc.png"></div>
<div class="card"><h3>Simulación</h3><ul><li>RoboDK</li></ul><img src="images/robodk.png"></div>
</div>

---

# Equipamiento previsto
<img class="logo-corner" src="images/tecnun_red.png" />

<div class="cards c3">
<div class="card"><h3>Robótica avanzada</h3><ul><li>Robot humanoide para docencia / investigación</li><li>Robot cuadrúpedo</li><li>Manos y grippers sensorizados</li></ul><div class="prio"><span class="dot alta"></span>PRIORIDAD ALTA</div></div>
<div class="card"><h3>Percepción e IA</h3><ul><li>Cámaras industriales</li><li>Sensores hápticos</li><li>Infraestructura GPU</li><li>Procesamiento de datos</li></ul><div class="prio"><span class="dot alta"></span>PRIORIDAD ALTA</div></div>
<div class="card"><h3>Laboratorio</h3><ul><li>Renovación de equipamiento obsoleto</li><li>Optimización del espacio para estudiantes</li><li>Infraestructura para investigación aplicada</li></ul><div class="prio"><span class="dot media"></span>PRIORIDAD MEDIA</div></div>
</div>

---

# Objetivos estratégicos
<img class="logo-corner" src="images/tecnun_red.png" />

<div class="goals">
<div class="goal"><div class="ic">👤</div><b>Talento</b>Captar talento investigador</div>
<div class="goal"><div class="ic">💻</div><b>Proyectos</b>Impulsar proyectos y colaboraciones</div>
<div class="goal"><div class="ic">🤖</div><b>Infraestructura</b>Modernizar laboratorio y equipamiento</div>
<div class="goal"><div class="ic">💡</div><b>Investigación</b>Impulsar robótica, visión e IA</div>
<div class="goal"><div class="ic">📖</div><b>Transferencia</b>Transferir tecnología a la industria</div>
</div>

<div class="mission">Consolidar un grupo multidisciplinar de referencia en robótica, automatización e inteligencia artificial, capaz de generar conocimiento, formar talento y transferir tecnología a la industria.</div>

---

<!-- _class: splash -->
<!-- _paginate: false -->
<!-- _footer: '' -->
<img src="images/tr_logo.png" alt="tecnun\ROBOTICS" />

---

# Club de Robótica
<img class="logo-corner" src="images/tecnun_red.png" />

<div class="lead" style="font-size: 26px;">

- Equipo de robótica de estudiantes de Tecnun, tutorizado por el grupo.
- Aplican robótica, electrónica, diseño mecánico e IA en proyectos reales con impacto social.

</div>

<div class="club">
<div>
<div class="item"><span class="dot ok"></span><b>R2-KT</b> · Robot para hospitales infantiles</div>
<div class="item"><span class="dot media"></span><b>Drones autónomos</b> · Navegación, visión artificial e IA</div>
<div class="item"><span class="dot alta"></span><b>Robótica de rescate</b> · Robots autónomos para entornos complejos</div>
<div style="font-size:18px"><span class="dot ok"></span>En marcha &nbsp; <span class="dot media"></span>En desarrollo &nbsp; <span class="dot alta"></span>Prevista</div>
</div>
<div class="robots">
<img src="images/r2kt.png"><img src="images/dron.png" style="height:120px"><img src="images/rescate.png" style="height:150px">
</div>
</div>

---

<!-- _class: cover -->
<!-- _backgroundColor: #e00000 -->
<!-- _backgroundImage: "radial-gradient(circle at 45% 100%, #ff2a2a 0%, #e00000 60%, #b80000 100%)" -->
<img class="cover-title" src="images/title_text.png" alt="Grupo de Robótica y Control" />
<img class="cover-logo" src="images/tecnun_white.png" alt="Tecnun Universidad de Navarra" />
<img class="cover-robot" style="height:62%" src="images/robot_final.png" alt="Robot" />
