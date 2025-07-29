---
# Using the penguin theme
theme: penguin
# apply any unocss classes to the current slide
class: 'text-center'
# https://sli.dev/custom/highlighters.html
highlighter: shiki
# show line numbers in code blocks
lineNumbers: false
# some information about the slides, markdown enabled
info: |
  ## LATN Slide Presentation
  
  A comprehensive presentation about the LATN project architecture, workflow, and implementation.
# persist drawings in exports and build
drawings:
  persist: false
# enable dark mode
colorSchema: 'dark'
# default transition between slides
transition: fade-out
# theme configuration for penguin
# themeConfig:
#   logoHeader: '/logo.svg'
#   twitter: '@latn_project'
#   twitterUrl: 'https://twitter.com/latn_project'
layout: intro
---
# LATN Project Presentation

A comprehensive overview of the LATN project architecture, workflow, and implementation

<div class="pt-12">
  <span @click="$slidev.nav.next" class="px-2 py-1 rounded cursor-pointer" hover="bg-white bg-opacity-10">
    Press Space for next page <carbon:arrow-right class="inline"/>
  </span>
</div>

---
src: ./sections/01-intro.md
---

---
src: ./sections/02-architecture.md
---

---
src: ./sections/03-workflow.md
---

---
src: ./sections/04-nginx-auth.md
---

---
src: ./sections/05-report.md
---

---
src: ./sections/06-conclusion.md
---
