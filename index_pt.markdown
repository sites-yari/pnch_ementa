---
layout: default
title: PNCH ementa - PT
class: index
---

<body>
  <!-- Main content -->
  <div class="pd-30">
    <div class="main_info col-md-12 ">
      <div class="text-center">
        <p class="ementa_title">{{site.data.ementa.pt.ementa_main_context.title}}</p>
      </div>
      <div>
        <p class="ementa_desc big_screen_organize">{{site.data.ementa.pt.ementa_main_context.desc}}</p>
      </div>
    </div>
  
    <!-- Menu -->
    <div class="main_info col-md-12 pd-20-top pd-30-bottom">
      <div class="main_divition_content"></div>
    </div>
    <div class="menu_content pd-10">
      <div class="big_screen_organize">
        <p class="ementa_title ementa_content">Ementa</p>
        <p class="ementa_desc">{{site.data.ementa.pt.menu.desc}}</p>
      </div>
    </div>
  
    <!-- a la carte -->
    {% include pt_menu.html %}
  
    <!-- snaks -->
    {% include pt_snacks.html %}
  
    <!-- Beverage -->
    {% include pt_beverage.html %}
  
    <!-- Wines -->
    {% include pt_wines.html %}


  <script>
    if (window.netlifyIdentity) {
      window.netlifyIdentity.on("init", user => {
        if (!user) {
          window.netlifyIdentity.on("login", () => {
            document.location.href = "/admin/";
          });
        }
      });
    }
  </script>
<!-- </body> -->
