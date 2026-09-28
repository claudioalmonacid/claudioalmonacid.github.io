# 🗺️ Mapa de Actores — Sistema Educacional Chileno

> **Fuente:** Documento 5 del Segundo Cerebro de Política Educacional  
> **Tipo:** Diagrama Mermaid · Renderiza nativamente en Obsidian

---

## Diagrama de actores y poder

```mermaid
graph TD
    subgraph ESTADO["⚙️ ESTADO Y ORGANISMOS INTERNACIONALES"]
        MIN["🏛️ MINEDUC\nPoder: Rector nacional\nF: Capital humano + Orden"]
        OCDE["🌐 OCDE / BM / UNESCO\nPoder: Técnico-normativo\nF: Capital humano + Equidad"]
    end

    subgraph POLITICA["🗳️ ACTORES POLÍTICOS"]
        DER["🔵 Bloque Derecha (Kast)\nPoder: Electoral + Gubernamental\nF: F5 Elección parental + F1 Orden\n2026: Gobierna"]
        IZQ["🔴 Bloque Izquierda (FA/PC/PS)\nPoder: Electoral + Técnico\nF: F4 Justicia + F2 Ciudadanía\n2026: Oposición"]
    end

    subgraph MERCADO["🏢 ACTORES DE MERCADO"]
        EMP["💼 Empresariado (SOFOFA/CPC)\nPoder: Ideológico + Lobby\nF: F3 Capital humano + F5 Valores mercado"]
        SOS["🏫 Sostenedores PS\nPoder: Electoral + Judicial\nF: F5 Libertad enseñanza + F3 Eficiencia"]
    end

    subgraph SOCIEDAD["✊ SOCIEDAD CIVIL"]
        DOC["📚 Colegio de Profesores\nPoder: Sindical + VETO\nF: F1 Transmisión cultural + F2 Cívica"]
        EST["🎓 Movimiento Estudiantil\nPoder: Movilización + Agenda\nF: F4 Igualdad. Anti-F5 segregación"]
        FAM["👨‍👩‍👧 Familias (actor difuso)\nPoder: Demanda mercado + Electoral\nF: F5 modo de vida + F4 movilidad"]
    end

    MIN --> DER
    MIN --> IZQ
    OCDE --> MIN
    EMP --> DER
    EMP --> SOS
    SOS --> DER
    DOC --> IZQ
    EST --> IZQ
    FAM --> DER
    FAM --> IZQ
    FAM --> SOS
```

---

## Actores con poder de VETO

```mermaid
graph LR
    V1["💼 Empresariado\nVeto ideológico + mediático\nNacional"]
    V2["📚 Colegio de Profesores\nVeto sindical\nNacional"]
    V3["🏫 Sostenedores PS\nVeto judicial + lobby\nNacional"]
    V4["⚖️ Tribunal Constitucional\nVeto judicial\nNacional"]
    V5["🗳️ Diputados independientes (40)\nVeto parlamentario\nLegislativo"]
    V6["👨‍👩‍👧 Familias\nVeto mercado - voto de pies\nLocal/nacional"]

    REFORMA["🔄 REFORMA\nEDUCACIONAL"] --> V1
    REFORMA --> V2
    REFORMA --> V3
    REFORMA --> V4
    REFORMA --> V5
    REFORMA --> V6
```

---

## Coaliciones históricas (1981–2026)

```mermaid
timeline
    title Coaliciones que gobernaron el sistema
    1981-1990 : Tecnócratas neoliberales + Militares
              : Voucher · Municipalización · LOCE
    1990-2005 : Tecnocracia Concertacionista + Empresariado
              : JEC · Salarios docentes · Sin cambio estructural
    2006-2010 : Pingüinos + Reformistas Concertación
              : LGE · SAC · Primera grieta al modelo
    2011-2014 : Movimiento estudiantil universitario
              : Agenda gratuidad · Fin al lucro · Base Bachelet II
    2014-2018 : Bachelet II + FA + Movimientos
              : Ley Inclusión · Carrera Docente · SLEP · Gratuidad
    2018-2021 : Piñera II - centroderecha
              : Sin contrarreforma estructural · Pandemia
    2021-2025 : Boric - FA + PC + PS
              : Crisis SLEP · FES aprobado · 2 plebiscitos fallidos
    2026-2030 : Kast - Derecha + Centroderecha
              : Mérito SAE · Escuelas Protegidas · Freno SLEP
```

---

*Nota: para el diagrama `timeline` necesitas Obsidian v1.4+ con Mermaid 10+*
