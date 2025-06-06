---
title: Projects - Zhaichanghao
display: Projects
description: List of projects that I am proud of
wrapperClass: 'text-center'
art: dots
projects:
  Current Focus:
    - name: "chz-cli"
      link: "https://github.com/KeyZhai/chz-cli"
      desc: 'a command line tool to create Vue and React project and template.'
      icon: 'i-tabler-tool'
    - name: 'MyBlog'
      link: 'https://github.com/KeyZhai/myBlog'
      desc: 'what you see is....'
      icon: 'i-game-icons-shark-jaws'
  Finished:
    - name: 'Core-cloud'
      link: 'https://github.com/KeyZhai/Core-Cloud'
      desc: 'a project based on Vue3 and Element-plus.'
      icon: 'i-iconamoon-cloud'
    - name: 'mini-vue'
      link: 'https://github.com/KeyZhai/MyVue'
      desc: 'Implemented the core functions of Vue.'
      icon: 'i-mingcute-vue-fill'
    - name: 'Cloud-Music'
      link: 'https://github.com/KeyZhai/Cloud-Music'
      desc: 'a project based on React and Ant Design.'
      icon: 'i-mdi-music'
    - name: 'ShishanClub'
      link: 'https://github.com/KeyZhai/ShiShanClub'
      desc: 'a project to show clubs and actitivies in HZAU'
      icon: 'i-lucide-mountain'
  Contribute:
    - name: 'Policy-Support-Platform'
      link: 'https://github.com/1071512987/policy_support_vue#readme'
      desc: 'A national intelligent support platform for agricultural policies.'
      icon: 'i-carbon-agriculture-analytics'
---

<!-- @layout-full-width -->
<ListProjects :projects="frontmatter.projects" />
