<template>
  <div class="container mt-5">
    <div class="row">
      <!-- Hero Section (Left Column) -->
      <div class="col-md-6 d-flex flex-column justify-content-center">
        <h1 class="display-4">Emi Shop</h1>
        <p class="lead">Discover, shop, and connect with Emi Shop! Our app combines the best of social media with the convenience of online shopping, creating a unique and engaging shopping experience.</p>
        <a class="d-none" href="https://play.google.com/store/apps/details?id=com.emicasolutions.emishopapp" target="_blank">
          <img src="/play.png" alt="Download on Play Store" class="img-fluid mt-3" style="max-width: 50%;"/>
        </a>
        <a href="/emishopapp.apk" target="_blank" download onclick="showFallback('viewer')">
          <img src="/download_apk.png" alt="Download APK" class="img-fluid mt-3" style="max-width: 50%;" />
        </a>
        <p id="fallback-viewer" class="fallback-message" style="display: none;">
          If the download doesn't start, <a href="/emishopapp.apk" target="_blank">click here</a> to download Location Viewer.
        </p>
      </div>

      <!-- Screenshots Section (Right Column) -->
      <div class="col-md-6">
        <div class="row">
          <div class="col-12 mb-4 justify-content-between screenshots">
            <img src="/detail.png" alt="Screenshot 1" class="img-fluid screenshot screenshot-t"/>
            <img src="/profile.png" alt="Screenshot 2" class="img-fluid screenshot screenshot-b" />
            <img src="/saved.png" alt="Screenshot 3" class="img-fluid screenshot screenshot-t"/>
            <img src="/new.png" alt="Screenshot 4" class="img-fluid screenshot screenshot-b"/>
          </div>
        </div>
      </div>
      
    </div>
  </div>
</template>

<style scoped>
/* Optional: Add custom styles here */
.hero-section {
  text-align: left;
}

.screenshot {
  max-width: 100%;
  height: auto;

}

.screenshot-t {
    margin-top: 50px;
}
.screenshot-b {
    margin-top: -50px;
}
.phone-mockup {
  position: relative;
  display: inline-block;
  width: 100%;
  max-width: 400px; /* Adjust based on the phone mockup size */
}

.phone-image {
  width: 100%;
  height: auto;
}

.screenshots {
  position: relative;
}

.screenshot {
  height: auto;
  width: 20%;
  margin-left: 20px;
  object-fit: fit;
  margin-bottom: 10px; /* Adjust spacing between screenshots */
  border-radius: 10px; /* Optional: Rounded corners for screenshots */
}

@media (max-width: 767px) {
  .screenshot {
  height: auto;
  width: 200px;
  object-fit: fit;
  margin-bottom: 10px; /* Adjust spacing between screenshots */
  border-radius: 10px; /* Optional: Rounded corners for screenshots */
  }
  .screenshot-t {
    margin-top: 20px;
}
.screenshot-b {
    margin-top: 20px;
}
}
</style>
