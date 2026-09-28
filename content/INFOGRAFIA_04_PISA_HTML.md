# 📊 Evidencia Empírica — Chile vs OCDE

> **Fuente:** Documento 4 del Segundo Cerebro de Política Educacional  
> **Tipo:** HTML embebido · Requiere plugin **Custom HTML** o **Obsidian HTML** en Obsidian

---

## Cómo usar este archivo

Para que el bloque HTML renderice en Obsidian necesitas instalar el plugin **"HTML Embed"** o **"Obsidian Custom HTML"** desde la tienda de plugins de la comunidad. Sin el plugin, verás el código HTML en texto plano.

---

```html
<style>
  .infografia {
    font-family: -apple-system, BlinkMacSystemFont, 'Segoe UI', sans-serif;
    background: #1e1e2e;
    color: #cdd6f4;
    border-radius: 12px;
    padding: 24px;
    max-width: 700px;
  }
  .titulo {
    font-size: 1.3em;
    font-weight: 700;
    color: #cba6f7;
    margin-bottom: 4px;
  }
  .subtitulo {
    font-size: 0.85em;
    color: #a6adc8;
    margin-bottom: 20px;
  }
  .seccion { margin-bottom: 24px; }
  .seccion-titulo {
    font-size: 0.9em;
    font-weight: 600;
    color: #89b4fa;
    text-transform: uppercase;
    letter-spacing: 1px;
    margin-bottom: 12px;
    border-bottom: 1px solid #313244;
    padding-bottom: 4px;
  }
  .barra-contenedor {
    display: flex;
    align-items: center;
    margin-bottom: 10px;
    gap: 10px;
  }
  .barra-label {
    font-size: 0.8em;
    width: 120px;
    flex-shrink: 0;
  }
  .barra-wrap {
    flex: 1;
    background: #313244;
    border-radius: 6px;
    height: 22px;
    position: relative;
    overflow: hidden;
  }
  .barra {
    height: 100%;
    border-radius: 6px;
    display: flex;
    align-items: center;
    justify-content: flex-end;
    padding-right: 8px;
    font-size: 0.75em;
    font-weight: 700;
    transition: width 1s ease;
  }
  .chile { background: linear-gradient(90deg, #f38ba8, #f38ba8cc); }
  .ocde  { background: linear-gradient(90deg, #89b4fa, #89b4facc); }
  .stat-grid {
    display: grid;
    grid-template-columns: repeat(3, 1fr);
    gap: 10px;
  }
  .stat-card {
    background: #313244;
    border-radius: 8px;
    padding: 12px;
    text-align: center;
  }
  .stat-numero {
    font-size: 1.6em;
    font-weight: 800;
    color: #f38ba8;
  }
  .stat-numero.bien { color: #a6e3a1; }
  .stat-label {
    font-size: 0.7em;
    color: #a6adc8;
    margin-top: 2px;
  }
  .leyenda {
    display: flex;
    gap: 16px;
    font-size: 0.78em;
    margin-bottom: 12px;
  }
  .leyenda span { display: flex; align-items: center; gap: 5px; }
  .dot { width: 10px; height: 10px; border-radius: 50%; display: inline-block; }
  .dot-chile { background: #f38ba8; }
  .dot-ocde  { background: #89b4fa; }
  .alerta {
    background: #45475a;
    border-left: 4px solid #f38ba8;
    border-radius: 4px;
    padding: 10px 14px;
    font-size: 0.82em;
    margin-top: 8px;
  }
  .ok {
    background: #45475a;
    border-left: 4px solid #a6e3a1;
    border-radius: 4px;
    padding: 10px 14px;
    font-size: 0.82em;
    margin-top: 8px;
  }
</style>

<div class="infografia">
  <div class="titulo">📊 Chile en evidencia — PISA 2022 y comparaciones OCDE</div>
  <div class="subtitulo">Segundo Cerebro · Política Educacional Chilena · Documento 4</div>

  <!-- PISA 2022 -->
  <div class="seccion">
    <div class="seccion-titulo">🌍 PISA 2022 — Puntajes Chile vs OCDE</div>
    <div class="leyenda">
      <span><span class="dot dot-chile"></span>Chile</span>
      <span><span class="dot dot-ocde"></span>OCDE Promedio</span>
    </div>

    <div class="barra-contenedor">
      <div class="barra-label">📖 Lectura</div>
      <div class="barra-wrap">
        <div class="barra chile" style="width:74%">448</div>
      </div>
    </div>
    <div class="barra-contenedor">
      <div class="barra-label"></div>
      <div class="barra-wrap">
        <div class="barra ocde" style="width:79%">476 OCDE</div>
      </div>
    </div>

    <div class="barra-contenedor" style="margin-top:8px">
      <div class="barra-label">🔬 Ciencias</div>
      <div class="barra-wrap">
        <div class="barra chile" style="width:73%">444</div>
      </div>
    </div>
    <div class="barra-contenedor">
      <div class="barra-label"></div>
      <div class="barra-wrap">
        <div class="barra ocde" style="width:80%">485 OCDE</div>
      </div>
    </div>

    <div class="barra-contenedor" style="margin-top:8px">
      <div class="barra-label">➗ Matemáticas</div>
      <div class="barra-wrap">
        <div class="barra chile" style="width:68%">412</div>
      </div>
    </div>
    <div class="barra-contenedor">
      <div class="barra-label"></div>
      <div class="barra-wrap">
        <div class="barra ocde" style="width:78%">472 OCDE</div>
      </div>
    </div>

    <div class="alerta">⚠️ <strong>56%</strong> de estudiantes chilenos de 15 años <strong>no alcanza el umbral mínimo</strong> de competencia matemática OCDE</div>
  </div>

  <!-- NiNis y cobertura -->
  <div class="seccion">
    <div class="seccion-titulo">👥 Cobertura y trayectorias</div>
    <div class="stat-grid">
      <div class="stat-card">
        <div class="stat-numero">26%</div>
        <div class="stat-label">NiNis 18–24 años<br><span style="color:#89b4fa">OCDE: 14,7%</span></div>
      </div>
      <div class="stat-card">
        <div class="stat-numero">75%</div>
        <div class="stat-label">Matrícula parvularia<br><span style="color:#89b4fa">OCDE: 85%</span></div>
      </div>
      <div class="stat-card">
        <div class="stat-numero">7%</div>
        <div class="stat-label">Sobreedad secundaria<br><span style="color:#89b4fa">OCDE: 4%</span></div>
      </div>
    </div>
    <div class="alerta">⚠️ Chile gasta <strong>más que OCDE</strong> en parvularia (0,70% PIB vs 0,60%) pero cubre <strong>menos niños</strong>. Problema de diseño, no de recursos.</div>
  </div>

  <!-- Educación superior -->
  <div class="seccion">
    <div class="seccion-titulo">🎓 Educación superior</div>
    <div class="stat-grid">
      <div class="stat-card">
        <div class="stat-numero">60%</div>
        <div class="stat-label">Financiamiento privado<br><span style="color:#89b4fa">OCDE: 30%</span></div>
      </div>
      <div class="stat-card">
        <div class="stat-numero">13%</div>
        <div class="stat-label">Gradúan en tiempo teórico<br><span style="color:#89b4fa">OCDE: 43%</span></div>
      </div>
      <div class="stat-card">
        <div class="stat-numero">2%</div>
        <div class="stat-label">Egresados con magíster<br><span style="color:#89b4fa">OCDE: 15%</span></div>
      </div>
    </div>
    <div class="alerta">⚠️ Solo <strong>1 de 8</strong> estudiantes chilenos termina su carrera en el tiempo establecido por el plan de estudios</div>
  </div>

  <!-- Opinión ciudadana -->
  <div class="seccion">
    <div class="seccion-titulo">💬 Opinión ciudadana (Cadem/Ipsos 2023-24)</div>
    <div class="stat-grid">
      <div class="stat-card">
        <div class="stat-numero">49%</div>
        <div class="stat-label">Califica el sistema de "malo" · Ipsos 2023</div>
      </div>
      <div class="stat-card">
        <div class="stat-numero bien">63%</div>
        <div class="stat-label">Apoya selección por mérito académico · Cadem 2024</div>
      </div>
      <div class="stat-card">
        <div class="stat-numero bien">61%</div>
        <div class="stat-label">Evalúa positivamente la ed. superior · Cadem 2024</div>
      </div>
    </div>
    <div class="ok">✅ El 63% pro-mérito es la <strong>base social del empate político</strong>: transversal a todos los signos, más fuerte que cualquier gobierno</div>
  </div>
</div>
```

---

## Alternativa sin plugin — tabla Markdown pura

| Indicador | Chile | OCDE | Brecha |
|---|---|---|---|
| PISA Lectura | 448 | 476 | -28 pts |
| PISA Ciencias | 444 | 485 | -41 pts |
| PISA Matemáticas | 412 | 472 | -60 pts |
| Bajo nivel mínimo Matemáticas | **56%** | 31% | +25pp |
| NiNis 18-24 años | **26%** | 14,7% | +11pp |
| Matrícula parvularia | 75% | 85% | -10pp |
| Graduación en tiempo teórico | 13% | 43% | -30pp |
| Egresados con magíster | 2% | 15% | -13pp |
| Financia. privado educación superior | 59,8% | 30% | +30pp |
| Apoya selección por mérito | 63% | — | Base empate político |
