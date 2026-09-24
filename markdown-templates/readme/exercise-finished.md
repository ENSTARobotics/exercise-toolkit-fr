{% set socials_text -%}
{%- if exercise_title -%}
Je viens de terminer l'exercice GitHub "{{ exercise_title }}" ! 🎉
{%- else -%}
Je viens de terminer un exercice GitHub interactif ! 🎉
{%- endif %}

{{ repository_url }}

#GitHubSkills #OpenSource #GitHubLearn
{%- endset -%}

<div align="center">

# 🎉 Félicitations {{ login }} ! 🎉

<img src="https://octodex.github.com/images/welcometocat.png" height="200px" />

### 🌟 Tu as terminé l'exercice avec succès ! 🌟

## 🚀 Partage ta réussite

**Tu peux partager ce que tu viens d'apprendre et le dépôt de l'exercice.**

<a href="https://twitter.com/intent/tweet?text={{ socials_text | urlencode }}" target="_blank" rel="noopener noreferrer">
  <img src="https://img.shields.io/badge/Partager%20sur%20X-1da1f2?style=for-the-badge&logo=x&logoColor=white" alt="Partager sur X" />
</a>
<a href="https://bsky.app/intent/compose?text={{ socials_text | urlencode }}" target="_blank" rel="noopener noreferrer">
  <img src="https://img.shields.io/badge/Partager%20sur%20Bluesky-0085ff?style=for-the-badge&logo=bluesky&logoColor=white" alt="Partager sur Bluesky" />
</a>
<a href="https://www.linkedin.com/feed/?shareActive=true&text={{ socials_text | urlencode }}" target="_blank" rel="noopener noreferrer">
  <img src="https://img.shields.io/badge/Partager%20sur%20LinkedIn-0077b5?style=for-the-badge&logo=linkedin&logoColor=white" alt="Partager sur LinkedIn" />
</a>

### 🎯 Et maintenant ?

[![](https://img.shields.io/badge/Revenir%20%C3%A0%20l'exercice-%E2%86%92-1f883d?style=for-the-badge&logo=github&labelColor=197935)]({{ issue_url }})
[![GitHub Skills](https://img.shields.io/badge/D%C3%A9couvrir%20GitHub%20Skills-000000?style=for-the-badge&logo=github&logoColor=white)](https://learn.github.com/skills)

*La meilleure façon d'apprendre reste de construire et d'expérimenter.* 🚀

</div>
