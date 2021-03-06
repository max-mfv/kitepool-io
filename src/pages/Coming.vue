<template>
  <video-bg :sources="['video/video.mp4']" img="img/placeholder.png">
    <!-- If you want to add content here, a slot is waiting! -->

    <div class="row">
      <div class="col-md-6 ml-auto mr-auto">
        <div class="c-container">
          <img class="brand-logo" src="img/brand_logo.png" alt="" />
          <h4 class="coming-title">Coming Soon</h4>
          <p class="c-description">Type something here</p>
          <fg-input
              class="no-border input-lg"
              addon-left-icon="now-ui-icons ui-1_email-85"
              placeholder="Enter you email"
            >
          </fg-input>
          <a
            href="#pablo"
            class="btn btn-primary btn-round btn-lg c-button"
            >Get access early</a
          >
        </div>
      </div>
      <div class="col-md-6 ml-auto mr-auto">
        <img class="n-logo" src="img/kitepool_logo_signle.png" alt="" />
      </div>
    </div>
  </video-bg>
</template>
<script>
import { Button, FormGroupInput } from '@/components';
export default {
  name: 'coming-page',
  bodyClass: 'coming-page',
  components: {
    [Button.name]: Button,
    [FormGroupInput.name]: FormGroupInput
  }
};
</script>
<style>

  .form-group.no-border .input-group-prepend .input-group-text, .input-group.no-border .input-group-prepend .input-group-text {
    color: white;
  }

  .n-logo {
    margin-top: 12%;
  }
  .c-container {
    margin-top: 12%;
    padding: 80px;
  }
  .brand-logo {
    height: 40px;
  }

  .coming-title {
    color: white;
    font-size: 40px;
    font-weight: bold;
  }
  .c-description {
    color: white;
    font-weight: bold;
  }
  .c-container .c-button {
    background-color: #2c2c2c;
    font-weight: bold;
  }
</style>

