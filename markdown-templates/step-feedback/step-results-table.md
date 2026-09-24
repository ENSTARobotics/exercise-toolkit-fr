{%- set all_passed = (results_table | selectattr("passed") | length) == (results_table | length) %}

{%- if all_passed %}

## Étape {{ step_number }} validée ✅

{%- else %}

## Étape {{ step_number }} à corriger ❌

{%- endif %}

{%- if all_passed %}
<img src="https://octodex.github.com/images/inflatocat.png" align="right" height="150px" alt="Étape validée" />
{%- else %}

<img src="https://octodex.github.com/images/spidertocat.png" align="right" height="100px" alt="Étape non validée" />

Certaines vérifications ont échoué. Consulte les résultats ci-dessous, corrige ce qui est nécessaire puis réessaie. 🤔
{%- endif %}

| Statut | Vérification |
| ------ | ------------ |

{%- for row in results_table %}
| {% if row.passed -%}✅ Validé{%- else -%}❌ À corriger{%- endif %} | {{ row.description }} |
{%- endfor %}

{%- if tips and tips.length %}

### Conseils

{%- for tip in tips %}

- {{ tip }}
  {%- endfor %}

{%- endif %}
