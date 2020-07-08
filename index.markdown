---
layout: default
title: PNCH ementa - EN
class: index
---

<body>
  <!-- Main content -->
  <div class="pd-30">
    <div class="main_info col-md-12 ">
      <div class="text-center">
        <p class="ementa_title">{{site.data.ementa.en.ementa_main_context.title}}</p>
      </div>
      <div>
        <p class="ementa_desc big_screen_organize">{{site.data.ementa.en.ementa_main_context.desc}}</p>
      </div>
    </div>
  
    <!-- Menu -->
    <div class="main_info col-md-12 pd-20-top pd-30-bottom">
      <div class="main_divition_content"></div>
    </div>
    <div class="menu_content pd-10">
      <div class="big_screen_organize">
        <p class="ementa_title ementa_content">Menu</p>
        <p class="ementa_desc">{{site.data.ementa.en.menu.desc}}</p>
      </div>
    </div>
  
    <!-- a la carte -->
    {% include en_menu.html %}
  
    <!-- snaks -->
    {% include en_snacks.html %}
  
    <!-- Beverage -->
    {% include en_beverage.html %}
  
    <!-- Wines -->
    {% include en_wines.html %}
  </div>


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
</body>
