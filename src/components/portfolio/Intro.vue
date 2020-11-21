<template lang="pug">
.p-intro.block-style
  .header.only-print
    //- h3 Candidate for
    span.last-updated Updated: August 8, 2019
  .image-row
    img.me(src="@/assets/me.jpg")
    p.only-print.qr-cta Scan this QR code to visit an online version of this resume
    img.qr(src="@/assets/qr.png")
  .profile-row
    .profile
      h1 Chaiyapat Tantiworachot
      h2 Solution Developer
      p: .
        A computer science student with a mixture of experience.
        Capable of working and leading in a team environment.
        Passionate about human-computer interaction and front-end development.
    .contact
      .single-contact
        span tel.
        span +66-81-5496692
      .single-contact
        span email.
        span chaiyapat@pix7.me
      .single-contact
        span in.
        span
          a.intro-link(href="https://linkedin.com/in/chaiyapat-t", target="_blank") linkedin.com/in/chaiyapat-t
      .single-contact
        span github.
        span
          a.intro-link(href="https://github.com/pixelart7", target="_blank") github.com/pixelart7
      .single-contact
        span site.
        span
          a.intro-link(href="https://pixelart7.github.io", target="_blank") pixelart7.github.io
          | ,
          |
          a.intro-link(href="https://pix7.me", target="_blank") pix7.me
</template>

<script>
export default {
};
</script>

<style lang="scss">
.p-intro {
  margin: 8px;
  margin-bottom: 0px;
  padding: 24px;
  .header {
    min-height: 36px;
    position: relative;
    color: #AAAAAA;
    span.last-updated {
      position: absolute;
      right: 0;
      color: #EEEEEE;
      font-size: 10px;
    }
  }
  .image-row {
    position: relative;
    .qr-cta {
      position: absolute;
      right: 76px + 12px;
      bottom: 0;
      width: 140px;
      margin: 0;
      text-align: right;
      font-size: 12px;
      color: #DDDDDD;
    }
    img {
      width: 76px;
      height: 76px;
      &.me {
        border-radius: 128px;
      }
      &.qr {
        position: absolute;
        justify-self: end;
        right: 0;
      }
    }
  }
  .profile-row {
    display: flex;
    .profile {
      flex: 2;
      padding-top: 12px;
      h1, h2 {
        margin-top: 0;
        margin-bottom: 4px;
      }
      p {
        margin-top: 8px;
        margin-bottom: 0;
      }
    }
    .contact {
      min-width: 180px;
      padding-top: 18px;
      padding-left: 12px;
      text-align: right;
      .single-contact {
        margin-bottom: 4px;
        span:first-child {
          margin-right: 12px;
          color: #BBBBBB;
        }
        span:last-child {
          font-weight: 500;
        }
      }
    }
    @media only screen and (max-width: 570px) {
      flex-direction: column;
      .contact {
        text-align: left;
        padding-left: 0;
        .single-contact span:first-child {
          display: inline-block;
          width: 64px;
        }
      }
    }
  }
}
</style>
