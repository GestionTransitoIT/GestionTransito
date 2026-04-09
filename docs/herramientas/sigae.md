---
layout: default
title: S.I.G.A.E
---

<div class="tool-hero">
  <h1>S.I.G.A.E</h1>
  <p class="tool-subtitle">
    Sistema Integral de Gestión y Administración de Entregas.
  </p>
  <p>
    Plataforma diseñada para la carga, seguimiento, control y liquidación de notificaciones, garantizando trazabilidad completa en cada etapa del proceso.
  </p>
</div>

---

## Descripción General

<div class="section-block">

S.I.G.A.E centraliza la gestión de notificaciones administrativas, permitiendo registrar, asignar y supervisar cada entrega realizada por los notificadores.

El sistema asegura trazabilidad operativa, control documental y transparencia en los procesos, incorporando además un módulo analítico y un sistema automatizado de liquidaciones.

</div>

---

## Gestión Operativa de Notificaciones

<div class="feature-grid">

<div class="feature-item">
<h3>Carga de Notificaciones</h3>
<p>Registro estructurado de datos asociados a cada notificación, incluyendo información del destinatario, domicilio y referencia administrativa.</p>
</div>

<div class="feature-item">
<h3>Asignación a Notificadores</h3>
<p>Distribución de notificaciones por usuario, con control de volumen y seguimiento individual de desempeño.</p>
</div>

<div class="feature-item">
<h3>Actualización de Estado</h3>
<p>Cambio automático de estado al momento de la entrega, garantizando control en tiempo real del proceso.</p>
</div>

<div class="feature-item">
<h3>Adjunto de Remito</h3>
<p>Incorporación de imagen digital del remito firmado como respaldo documental de cada notificación entregada.</p>
</div>

</div>

---

## Trazabilidad y Control

<div class="section-block">

<h3>Registro de Operaciones</h3>
<p>Cada acción realizada dentro del sistema queda almacenada, permitiendo auditoría completa sobre modificaciones, entregas y actualizaciones.</p>

<h3>Historial por Notificación</h3>
<p>Seguimiento detallado del ciclo de vida de cada notificación desde su carga inicial hasta su cierre definitivo.</p>

<h3>Control de Usuarios</h3>
<p>Gestión de perfiles y permisos para asegurar integridad y responsabilidad operativa.</p>

</div>

---

## Módulo Analítico

<div class="section-block">

<h3>Indicadores de Entrega</h3>
<p>Métricas sobre volumen de notificaciones asignadas, entregadas, pendientes y rechazadas.</p>

<h3>Rendimiento por Notificador</h3>
<p>Análisis comparativo del desempeño individual y productividad operativa.</p>

<h3>Estadísticas Temporales</h3>
<p>Visualización de actividad por períodos diarios, semanales o mensuales para optimización de recursos.</p>

</div>

---

## Módulo de Liquidación

<div class="section-block">

<h3>Cálculo Automatizado</h3>
<p>Determinación automática del importe correspondiente a cada notificador según entregas registradas y criterios configurados.</p>

<h3>Resumen de Pagos</h3>
<p>Visualización consolidada de montos a liquidar por período.</p>

<h3>Transparencia y Control</h3>
<p>Acceso a detalle de cada notificación incluida en la liquidación para garantizar precisión y trazabilidad.</p>

</div>
## Vista del Producto

<div class="image-grid">
  <div class="image-card">
    <img src="{{ '/assets/img/SIGAEindex.png' | relative_url }}" alt="Pagina Principal">
    <h4>Pagina Principal</h4>
  </div>
  <div class="image-card">
    <img src="{{ '/assets/img/SIGAEload.png' | relative_url }}" alt="Carga">
    <h4>Carga</h4>
  </div>
  <div class="image-card">
    <img src="{{ '/assets/img/SIGAEtable.png' | relative_url }}" alt="Listado de Notificaciones">
    <h4>Listado de Notificaciones</h4>
  </div>
  <div class="image-card">
    <img src="{{ '/assets/img/SIGAEquery.png' | relative_url }}" alt="Consulta">
    <h4>Consulta</h4>
  </div>
</div>

<!-- LIGHTBOX -->
<div id="lightbox" class="lightbox">
  <span class="close">&times;</span>
  <img class="lightbox-img">
</div>

<style>
.image-grid {
  display: grid;
  grid-template-columns: repeat(2, 1fr);
  gap: 20px;
  margin-top: 20px;
}

.image-card {
  text-align: center;
}

.image-card img {
  width: 100%;
  cursor: pointer;
  border-radius: 8px;
  transition: transform 0.2s;
}

.image-card img:hover {
  transform: scale(1.03);
}

.image-card h4 {
  margin-top: 8px;
  font-weight: 500;
}

.lightbox {
  display: none;
  position: fixed;
  z-index: 999;
  top: 0;
  left: 0;
  width: 100%;
  height: 100%;
  background: rgba(0,0,0,0.8);
  justify-content: center;
  align-items: center;
}

.lightbox-img {
  max-width: 90%;
  max-height: 90%;
}

.close {
  position: absolute;
  top: 20px;
  right: 30px;
  color: #fff;
  font-size: 40px;
  cursor: pointer;
}
</style>

<script>
document.addEventListener("DOMContentLoaded", function() {
  const images = document.querySelectorAll(".image-card img");
  const lightbox = document.getElementById("lightbox");
  const lightboxImg = document.querySelector(".lightbox-img");
  const closeBtn = document.querySelector(".close");

  images.forEach(img => {
    img.addEventListener("click", () => {
      lightbox.style.display = "flex";
      lightboxImg.src = img.src;
    });
  });

  function closeLightbox() {
    lightbox.style.display = "none";
  }

  closeBtn.addEventListener("click", closeLightbox);

  lightbox.addEventListener("click", (e) => {
    if (e.target !== lightboxImg) closeLightbox();
  });

  document.addEventListener("keydown", (e) => {
    if (e.key === "Escape") closeLightbox();
  });
});
</script>
