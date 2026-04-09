---
layout: default
title: Inicio
---
<section id="proyectos" class="section">
  <h2>Proyectos</h2>

  <div class="project-grid">

    <!-- PROYECTO TESSA -->
    <div class="project-card">
      <img src="{{ '/assets/img/Dashindex.png' | relative_url }}" alt="TESSA Dashboard">
      <div class="project-content">
        <h3>T.E.S.S.A</h3>
        <p>
          Plataforma de análisis y monitoreo de fiscalización de fotomultas, 
          con métricas operativas, visualizaciones dinámicas y seguimiento de rendimiento.
        </p>
        <div class="project-tech">
          <span>Python</span>
          <span>Streamlit</span>
          <span>Pandas</span>
          <span>Data Visualization</span>
        </div>

        <div class="project-actions">
          <a href="{{ 'herramientas/tessa' | relative_url }}" class="btn primary">
            Ver detalle
          </a>

          <a href="https://aset.unlam.edu.ar/tessa/" class="btn secondary" target="_blank">
            Ingresar
          </a>
        </div>
      </div>
    </div>

    <!-- WEB SCRAPING -->
    <div class="project-card">
      <img src="{{ '/assets/img/webscrapcaptura.jpg' | relative_url }}" alt="Web Scraping">
      <div class="project-content">
        <h3>Web Scraping App</h3>
        <p>Sistema de extracción y procesamiento automático de datos desde múltiples fuentes.</p>
        <div class="project-tech">
          <span>Python</span>
          <span>BeautifulSoup</span>
          <span>Automation</span>
        </div>

        <div class="project-actions">
          <a href="{{ 'herramientas/tai' | relative_url }}" class="btn primary">
            Ver detalle
          </a>

          <a href="#" class="btn secondary">
            Ingresar
          </a>
        </div>
      </div>
    </div>

    <!-- ACTIVIDAD MUNICIPAL -->
    <div class="project-card">
      <img src="{{ '/assets/img/Login.png' | relative_url }}" alt="Login">
      <div class="project-content">
        <h3>Actividad Municipal App</h3>
        <p>Dashboard interactivo sobre la actividad de fotomultas en un municipio. Desarrollado exclusivamente para la Universidad de La Matanza</p>
        <div class="project-tech">
          <span>Python</span>
          <span>Visualizacion</span>
          <span>Data Analytics</span>
        </div>

        <div class="project-actions">
          <a href="{{ 'herramientas/berys' | relative_url }}" class="btn primary">
            Ver detalle
          </a>

          <a href="#" class="btn secondary">
            Ingresar
          </a>
        </div>
      </div>
    </div>

  </div>
</section>
