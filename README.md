<!DOCTYPE html><html lang="es">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Malla Curricular - Imagenología</title>
  <style>
    body {
      font-family: sans-serif;
      background: #f8f9fa;
      margin: 2rem;
      text-align: center;
    }
    h1 {
      margin-bottom: 1rem;
    }
    .year {
      font-size: 1.5rem;
      margin: 1rem 0 0.5rem;
      color: #333;
    }
    .grid {
      display: grid;
      grid-template-columns: repeat(auto-fit, minmax(200px, 1fr));
      gap: 1rem;
      margin-bottom: 2rem;
    }
    .subject {
      padding: 1rem;
      border-radius: 8px;
      background: #ffffff;
      box-shadow: 0 2px 5px rgba(0, 0, 0, 0.1);
      cursor: pointer;
      transition: 0.3s;
    }
    .subject.approved {
      background: #d4edda;
      text-decoration: line-through;
    }
    .subject.in-progress {
      background: #fff3cd;
    }
    .subject.pending {
      background: #f8d7da;
    }
  </style>
</head>
<body>
  <h1>Malla Curricular - Imagenología (EUTM)</h1>  <div class="year">Primer Año</div>
  <div class="grid">
    <div class="subject pending">Anatomía</div>
    <div class="subject pending">Biología Celular y Tisular</div>
    <div class="subject pending">Neurobiología</div>
    <div class="subject pending">Cardio Vascular y Respiratorio</div>
    <div class="subject pending">Digestivo Renal y Endocrino</div>
    <div class="subject pending">Reproductor y Desarrollo</div>
    <div class="subject pending">Enfermería</div>
    <div class="subject pending">Psicología I</div>
    <div class="subject pending">Física Básica</div>
    <div class="subject pending">Salud Pública</div>
    <div class="subject pending">Metodología Científica</div>
    <div class="subject pending">Fisiopatología</div>
    <div class="subject pending">Física Radiológica</div>
  </div>  <div class="year">Segundo Año</div>
  <div class="grid">
    <div class="subject pending">Técnicas Radiológicas I</div>
    <div class="subject pending">Protección Radiológica y Control de Calidad</div>
    <div class="subject pending">Anatomía Radiológica I</div>
    <div class="subject pending">Sistema de Procesamiento de Imagen I</div>
    <div class="subject pending">Anatomía Radiológica II</div>
    <div class="subject pending">Sistema de Procesamiento de Imagen II</div>
    <div class="subject pending">Técnicas Radiológicas II</div>
  </div>  <div class="year">Tercer Año</div>
  <div class="grid">
    <div class="subject pending">Anatomía Radiológica III</div>
    <div class="subject pending">Técnicas Radiológicas III</div>
    <div class="subject pending">Imagenología Especializada I</div>
    <div class="subject pending">Introducción al Trabajo Científico</div>
    <div class="subject pending">Deontología y Legislación Laboral</div>
    <div class="subject pending">Administración Hospitalaria</div>
  </div>  <div class="year">Cuarto Año</div>
  <div class="grid">
    <div class="subject pending">Imagenología Especializada II</div>
    <div class="subject pending">Internado</div>
    <div class="subject pending">Monografía</div>
    <div class="subject pending">Seminarios Académicos del Hospital de Clínicas</div>
  </div>  <script>
    document.querySelectorAll('.subject').forEach(subject => {
      subject.addEventListener('click', () => {
        if (subject.classList.contains('pending')) {
          subject.classList.remove('pending');
          subject.classList.add('in-progress');
        } else if (subject.classList.contains('in-progress')) {
          subject.classList.remove('in-progress');
          subject.classList.add('approved');
        } else if (subject.classList.contains('approved')) {
          subject.classList.remove('approved');
          subject.classList.add('pending');
        }
      });
    });
  </script></body>
</html>
