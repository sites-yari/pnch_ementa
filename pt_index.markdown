---
layout: default
title: PNCH ementa - PT
class: index
---

<body>
  <!-- Main content -->
  <div class="pd-30">
    <div class="main_info col-md-12 bg_lgrey">
      <div class="text-center">
        <p class="ementa_title">{{site.data.ementa.pt.ementa_main_context.title}}</p>
      </div>
      <div>
        <p class="ementa_desc">{{site.data.ementa.pt.ementa_main_context.desc}}</p>
      </div>
    </div>
  
    <!-- Menu -->
    <div class="main_info col-md-12 pd-20-top pd-30-bottom">
      <div class="main_divition_content"></div>
    </div>
    <div class="menu_content pd-10">
      <div class="bg_lgrey">
        <p class="ementa_title ementa_content">Menu</p>
        <p class="ementa_title">{{site.data.ementa.pt.menu.title}}</p>
        <p class="ementa_desc">{{site.data.ementa.pt.menu.desc}}</p>
      </div>
    </div>
  
    <!-- a la carte -->
    <div class="main_info col-md-12 pd-10-top pd-10-bottom">
      <div class="divition_content"></div>
    </div>
    <div class="la_carte_content pd-10">
      <div class="bg_lgrey">
        <p class="ementa_title ementa_content">A la Carte</p>
        <!-- starter -->
        <div>
          <p class="ementa_desc_important mrg-0">Starter</p>
          <p class="ementa_desc">{{site.data.ementa.pt.la_carte.starter}}</p>
        </div>
        <!-- appetizers -->
        <div>
          <p class="ementa_desc_important mrg-0">Appetizers</p>
          <p class="ementa_desc">{{site.data.ementa.pt.la_carte.appetizer}}</p>
        </div>
        <!-- fish -->
        <div>
          <p class="ementa_desc_important mrg-0">Fish</p>
          <p class="ementa_desc">{{site.data.ementa.pt.la_carte.fish}}</p>
        </div>
        <!-- meat -->
        <div>
          <p class="ementa_desc_important mrg-0">Meat</p>
          <p class="ementa_desc">{{site.data.ementa.pt.la_carte.meat}}</p>
        </div>
        <!-- vegetarian -->
        <div>
          <p class="ementa_desc_important mrg-0">Vegetarian</p>
          <p class="ementa_desc">{{site.data.ementa.pt.la_carte.vegetarian}}</p>
        </div>
        <!-- childs menu -->
        <div>
          <p class="ementa_desc_important mrg-0">Children's menu</p>
          <p class="ementa_desc">{{site.data.ementa.pt.la_carte.childrens_menu}}</p>
        </div>
        <!-- dessert -->
        <div>
          <p class="ementa_desc_important mrg-0">Dessert</p>
          <p class="ementa_desc">{{site.data.ementa.pt.la_carte.desert}}</p>
        </div>
        <!-- extra info -->
        <div>
          <p class="ementa_desc">{{site.data.ementa.pt.la_carte.extra_info}}</p>
        </div>
      </div>
    </div>
  
    <!-- snaks -->
    <div class="main_info col-md-12 pd-10-top pd-10-bottom">
      <div class="divition_content"></div>
    </div>  
    <div class="snacks_content pd-10">
      <div class="bg_lgrey">
        <p class="ementa_title ementa_content">Snacks</p>
        <p class="ementa_title">{{site.data.ementa.pt.snacks.title}}</p>
        <p class="ementa_desc">{{site.data.ementa.pt.snacks.desc}}</p>
      </div>
    </div>
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
