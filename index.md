---
title: Home
layout: default.html
---

<article>
  <h2>Regulamentação</h2>
  <p>
    Placas já encontradas (<b>{{ placas.R | size }}</b>&nbsp;/&nbsp;59?):
  </p>
  <ul>
  {%- for placa in placas.R -%}
    <li>
      <figure>
        <figcaption>
          <h3>R-{{ placa.id }}</h3>
          <p>{{ placa.name }}</p>
        </figcaption>
        <img src="placas/R{{ placa.file }}.jpg">
      </figure>
    </li>
  {%- endfor -%}
  </ul>
  <p>Placas ainda não encontradas:</p>
  <ul>
  {%- for placa in placas.R_total -%}
    <li>
      <figure class="faltante">
        <figcaption>
          <h3>R-{{ placa }}</h3>
        </figcaption>
        <img src="placas/falta/R{{ placa }}.png">
      </figure>
    </li>
  {%- endfor -%}
  </ul>
</article>
<hr>
<article>
  <h2>Advertência</h2>
  <p>
    Placas já encontradas: (<b>{{ placas.A | size }}</b>&nbsp;/&nbsp;69?)
  </p>
  <ul>
  {%- for placa in placas.A -%}
    <li>
      <figure>
        <figcaption>
          <h3>A-{{ placa.id }}</h3>
          <p>{{ placa.name }}</p>
        </figcaption>
        <img src="placas/A{{ placa.file }}.jpg">
      </figure>
    </li>
  {%- endfor -%}
  </ul>
  <p>Placas ainda não encontradas:</p>
  <ul>
  {%- for placa in placas.A_total -%}
    <li>
      <figure class="faltante">
        <figcaption>
          <h3>A-{{ placa }}</h3>
        </figcaption>
        <img src="placas/falta/A{{ placa }}.png">
      </figure>
    </li>
  {%- endfor -%}
  </ul>
</article>