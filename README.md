# product-page-tab-shopify
This code will work to make the tabs in product page


Here is the Script for Activation add this Script to theme.liquid file
<script>
  $('ul.tabs li').click(function(){
     var tab_id = $(this).attr('data-tab');

     $('ul.tabs li').removeClass('current');
     $('.tab-content').removeClass('current');

     $(this).addClass('current');
     $("#"+tab_id).addClass('current');
   })
 </script>
