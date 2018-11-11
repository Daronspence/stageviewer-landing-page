<template>
  <div class="sign-up">
    <!-- Begin Mailchimp Signup Form -->
    <div id="mc_embed_signup" class="text-left mx-auto">
    <form action="https://acfwidgets.us9.list-manage.com/subscribe/post?u=66c6af09ba208080a03459801&amp;id=dc648e2428" method="post" id="mc-embedded-subscribe-form" name="mc-embedded-subscribe-form" class="validate" target="_blank" novalidate>
      <div id="mc_embed_signup_scroll">

    <div class="indicates-required text-xs text-red text-left mb-1"><span class="asterisk">*</span> required</div>
    <div class="flex mb-4 flex-col sm:flex-row items-center">
      <label for="mce-EMAIL" class="flex-1">Email Address  <span class="asterisk text-red">*</span></label>
      <input type="email" value="" required name="EMAIL" class="required email px-4 py-2 border" id="mce-EMAIL">
    </div>
    <div class="flex mb-4 flex-col sm:flex-row items-center">
      <label for="mce-FNAME" class="flex-1">First Name </label>
      <input type="text" value="" name="FNAME" class="px-4 py-2 border" id="mce-FNAME">
    </div>
    <div class="flex mb-4 flex-col sm:flex-row items-center">
      <label for="mce-LNAME" class="flex-1">Last Name </label>
      <input type="text" value="" name="LNAME" class="px-4 py-2 border" id="mce-LNAME">
    </div>
    <div id="mce-responses" class="clear">
      <div class="response" id="mce-error-response" style="display:none"></div>
      <div class="response" id="mce-success-response" style="display:none"></div>
    </div>    <!-- real people should not fill this in and expect good things - do not remove this or risk form bot signups-->
      <div style="position: absolute; left: -5000px;" aria-hidden="true"><input type="text" name="b_66c6af09ba208080a03459801_dc648e2428" tabindex="-1" value=""></div>
      <div class="text-center mt-8"><input type="submit" value="Subscribe to Updates" name="subscribe" id="mc-embedded-subscribe" class="p-2 bg-green-dark text-white"></div>
      </div>
    </form>
    </div>
    <!--End mc_embed_signup-->
  </div>
</template>

<script>
export default {
  props: {
    msg: String
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>

</style>
