<template>
  <div class="container">
    <main class="card">
      <div class="qr-container">
        <img class="qr-image" src="./assets/qr-code.png" alt="Frontendmentor QR Code">
      </div>
      <div class="content">
      <h1 class="title">Improve your front-end skills by building projects</h1>
        <p class="description">Scan the QR code to visit Frontend Mentor and take your coding skills to the next level</p>
      </div>
    </main>
  </div>
</template>

<style scoped>
.container {
  display: flex;
  flex-direction: column;
  justify-content: center;
  align-items: center;
  flex: 1;
  padding: 0 28px;
}

.card {
  display: flex;
  flex-direction: column;
  border-radius: 20px;
  background-color: var(--white);
  width: 320px;
  box-shadow: 0 25px 25px rgba(0, 0, 0, 0.0476518);
  padding: 16px;
}

.qr-container {
  width: 100%;
  height: 288px;
  margin-bottom: 24px;
}

.qr-image {
  width: 100%;
  height: 100%;
  border-radius: 10px;
}

.content {
  text-align: center;
}

.title {
  font-size: 1.375rem;
  color: var(--dark-navy);
  line-height: 28px;
  font-weight: 700;
}

.description {
  font-size: 0.9375rem;
  color: var(--grey);
  line-height: 19px;
  letter-spacing: 0.1875px;
  padding: 16px 16px 24px 16px;
}
</style>