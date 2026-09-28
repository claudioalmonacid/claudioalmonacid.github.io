# 🧠 Marco Teórico — Collins · Hopper · Peña

> **Fuente:** Documento 2 del Segundo Cerebro de Política Educacional  
> **Tipo:** Diagrama Mermaid · Renderiza nativamente en Obsidian

---

## Las 5 funciones del sistema educacional (Hopper/Peña)

```mermaid
graph TD
    SIS["🏫 SISTEMA EDUCACIONAL\nCHILENO"] --> F1 & F2 & F3 & F4 & F5

    F1["🎭 F1 — SOCIOCULTURAL\nTransmitir conciencia\nmoral y cultural compartida"]
    F2["🗳️ F2 — POLÍTICA/CÍVICA\nFormar ciudadanos\npara la democracia"]
    F3["⚙️ F3 — CAPITAL HUMANO\nProveer competencias\nproductivas y técnicas"]
    F4["⚖️ F4 — JUSTICIA/IGUALDAD\nBorrar la cuna:\nel destino no depende del origen"]
    F5["🏠 F5 — MODO DE VIDA\nFamilias transmiten\nsus valores por la escuela"]

    F4 <-->|"⚡ TENSIÓN CENTRAL\nEmpate político chileno"| F5

    style F4 fill:#339af0,color:#fff,stroke:#1c7ed6
    style F5 fill:#f03e3e,color:#fff,stroke:#c92a2a
    style F4 stroke-width:3px
    style F5 stroke-width:3px
```

---

## Tríada de demandas de Collins

```mermaid
graph LR
    subgraph COLLINS["🔺 TRÍADA DE COLLINS — Origen de las demandas educativas"]
        CL["💰 Demanda de CLASE\nHabilidades prácticas\nAprendizaje funcional\n→ EMTP chilena"]
        ES["👑 Demanda de ESTAMENTO\nMembresía simbólica\nRituales de distinción\n→ Colegios de élite · inglés · deportes de nicho"]
        BU["📋 Demanda de BUROCRACIA\nCredenciales formales\nEl contenido es secundario\n→ Expansión universitaria · carreras baratas"]
    end

    CL --- ES
    ES --- BU
    BU --- CL

    INFLACION["📈 INFLACIÓN DE CREDENCIALES\nLo que antes requería secundaria\nahora exige licenciatura"] -.-> BU

    style CL fill:#51cf66,color:#fff
    style ES fill:#ffd43b,color:#333
    style BU fill:#74c0fc,color:#333
```

---

## El Proceso de Selección Total (Hopper)

```mermaid
flowchart TD
    PST["🔄 PROCESO DE SELECCIÓN TOTAL\nCómo la sociedad decide quién sube,\nquién se queda y cómo gestiona la frustración"]

    PST --> EN["1️⃣ ENTRENAMIENTO\nHabilidades técnicas y normativas\npara roles adultos\n\n🇨🇱 Chile: EMTP entrena roles técnicos\npero no transmite códigos culturales\ndel estrato al que se aspira"]

    PST --> SE["2️⃣ SELECCIÓN\nIdentificar y categorizar personas\nsegún habilidades\n\n🇨🇱 Chile: PAES y SIMCE miden\nrendimiento acumulado, no talento puro\n→ Reproducen el origen social"]

    PST --> AS["3️⃣ ASIGNACIÓN\nColocar personal calificado\nen roles ocupacionales\n\n🇨🇱 Chile: Sobreoferta de egresados\nsin empleos calificados disponibles\n→ Desajuste credencial/empleo"]

    PST --> RC["4️⃣ REGULACIÓN DE LA AMBICIÓN\nCalentamiento y enfriamiento:\ncontrolar deseos según vacantes reales\n\n🇨🇱 Chile: CALIENTA eficientemente\nENFRÍA MAL → 26% NiNis\n→ Combustible del conflicto político"]

    EN --> FALLA["🚨 DISFUNCIÓN SISTÉMICA\nChile falla en los\n4 sub-problemas simultáneamente"]
    SE --> FALLA
    AS --> FALLA
    RC --> FALLA

    style RC fill:#ff6b6b,color:#fff,stroke-width:3px
    style FALLA fill:#f03e3e,color:#fff
```

---

## Calentamiento y enfriamiento: el ciclo fallido

```mermaid
sequenceDiagram
    participant SIS as 🏫 Sistema Educacional
    participant FAM as 👨‍👩‍👧 Familias
    participant MER as 💼 Mercado Laboral
    participant POL as 🔥 Conflicto Político

    SIS->>FAM: CALENTAMIENTO: promesa de movilidad social
    FAM->>SIS: Demanda masiva de títulos universitarios
    SIS->>MER: Entrega credenciales (deuda CAE + años)
    MER->>FAM: ❌ Empleo precario / no acorde al título
    Note over FAM,MER: Brecha entre expectativa y realidad
    FAM->>POL: Frustración politizada
    Note over POL: 2006 Pingüinos · 2011 Universitarios · 2019 Estallido
    SIS-->>FAM: ❓ Enfriamiento fallido: sin rutas alternativas dignas
```

---

## Ideologías de selección (Hopper expandido de Turner)

```mermaid
quadrantChart
    title Tipos de sistema según Hopper
    x-axis "Selección TEMPRANA" --> "Selección TARDÍA"
    y-axis "PARTICULARISTA (adscriptivo)" --> "UNIVERSALISTA (mérito)"
    quadrant-1 Concurso tardío-universal
    quadrant-2 Concurso temprano-universal
    quadrant-3 Patrocinio temprano-particular
    quadrant-4 Patrocinio tardío-particular
    Chile declarado: [0.75, 0.8]
    Chile real: [0.25, 0.3]
    Europa continental: [0.15, 0.65]
    EE.UU.: [0.85, 0.75]
```

> **Chile:** declara movilidad por **concurso** (PAES abierta, mérito individual) pero opera con movilidad **patrocinada encubierta** (preuniversitarios, redes, capital cultural).
