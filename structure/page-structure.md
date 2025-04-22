# 📄 Page Structure



{% tabs %}
{% tab title="HTML" %}
```html
<!DOCTYPE html>
<html lang="en">
  <!-- [Head] start -->

  <head>
    <title>Dashboardkit Dashboard Template</title>
    <!-- [Meta] -->
    <meta charset="utf-8" />
    <meta name="viewport" content="width=device-width, initial-scale=1.0, user-scalable=0, minimal-ui"/>
    <meta http-equiv="X-UA-Compatible" content="IE=edge" />
    <meta name="description" content="" />
    <meta name="keywords" content="" />
    <meta name="author" content="" />

    <!-- [Favicon] icon -->
    <link rel="icon" href="../assets/images/favicon.svg" type="image/x-icon" />
    <!-- [Google Font : Public Sans] icon -->
    <link href="https://fonts.googleapis.com/css2?family=Inter:wght@700..700&display=swap" rel="stylesheet"/>

    <!-- [Tabler Icons] https://tablericons.com -->
    <link rel="stylesheet" href="../assets/fonts/tabler-icons.min.css" />
    <!-- [Feather Icons] https://feathericons.com -->
    <link rel="stylesheet" href="../assets/fonts/feather.css" />
    <!-- [Font Awesome Icons] https://fontawesome.com/icons -->
    <link rel="stylesheet" href="../assets/fonts/fontawesome.css" />
    <!-- [Material Icons] https://fonts.google.com/icons -->
    <link rel="stylesheet" href="../assets/fonts/material.css" />
    <!-- [Template CSS Files] -->
    <link rel="stylesheet" href="../assets/css/style.css" id="main-style-link"/>
    <link rel="stylesheet" href="../assets/css/style-preset.css" />
  </head>
  <!-- [Head] end -->
  <!-- [Body] Start -->

  <body data-pc-preset="preset-1" data-pc-sidebar-theme="dark" data-pc-header-theme="light" data-pc-sidebar-caption="true" data-pc-direction="ltr" data-pc-theme="light">
  
    <!-- [ Pre-loader ] start -->
    <div class="loader-bg">
    </div>
    <!-- [ Pre-loader ] End -->
    
    <!-- [ Sidebar Menu ] start -->
    <nav class="pc-sidebar">
    </nav>
    <!-- [ Sidebar Menu ] end -->
    
    <!-- [ Header Topbar ] start -->
    <header class="pc-header">
    </header>
    <!-- [ Header ] end -->

    <!-- [ Main Content ] start -->
    <div class="pc-container">
      <div class="pc-content">
      
        <!-- [ breadcrumb ] start -->
        <div class="page-header">
        </div>
        <!-- [ breadcrumb ] end -->

        <!-- [ Main Content ] start -->
        <div class="row">
        </div>
        <!-- [ Main Content ] end -->
        
      </div>
    </div>
    <!-- [ Main Content ] end -->
    
    <footer class="pc-footer">
    </footer>
    
    <!-- Required Js -->
    <script src="../assets/js/plugins/popper.min.js"></script>
    <script src="../assets/js/plugins/simplebar.min.js"></script>
    <script src="../assets/js/plugins/bootstrap.min.js"></script>
    <script src="../assets/js/fonts/custom-font.js"></script>
    <script src="../assets/js/pcoded.js"></script>
    <script src="../assets/js/plugins/feather.min.js"></script>
  </body>
  <!-- [Body] end -->
</html>

```
{% endtab %}

{% tab title="GULP" %}
```html
<!doctype html>
<html lang="en">

  <!-- [Head] start -->
  <head>
    @@include('../layouts/head-page-meta.html', {'title': 'Sample Page'})
    @@include('../layouts/head-css.html')
  </head>
  <!-- [Head] end -->
  
  <!-- [Body] Start -->
  <body @@bodySetup>
    @@include('../layouts/layout-vertical.html')

    <!-- [ Main Content ] start -->
    <div class="pc-container">
      <div class="pc-content">
        @@include('../layouts/breadcrumb.html', {'breadcrumb-item': 'Other', 'breadcrumb-item-active': 'Sample Page'})

        <!-- [ Main Content ] start -->
        <div class="row">
        </div>
        <!-- [ Main Content ] end -->
      </div>
    </div>
    <!-- [ Main Content ] end -->
    @@include('../layouts/footer-block.html')
    @@include('../layouts/footer-js.html')
    @@include('../layouts/customizer.html')
  </body>
  <!-- [Body] end -->
</html>

```
{% endtab %}
{% endtabs %}
