<template lang="pug">
#app
  .fullpage#fullpage(ref="fullpage")
    .overlay(@click="collapse")
    router-view
</template>

<script>
export default {
  methods: {
    collapse() {
      this.$router.push({ name: 'home' });
    },
  },
};
</script>

<style lang="scss">
@import url('~sanitize.css');

$bg: #0ED2F7;
$border-radius: 8px;

$image-slide-height: 360px;

body, html {
  width: 100%;
  color: #333333;
  background: $bg;
  // background: #333333;
}

a:not(.intro-link) {
  color: darken($bg, 15);
  transition: color 0.15s;
  &:hover {
    color: darken($bg, 10);
  }
  &.non-cta {
    color: #333333;
    text-decoration: none;
    border-bottom: 1px solid rgba(#000000, 0.15);
    &:hover {
      color: darken($bg, 10);
      border-color: darken($bg, 10);
    }
  }
  &[target="_blank"] {
    position: relative;
    &:after {
      opacity: 0;
      display: inline-block;
      position: absolute;
      margin-top: 2px;
      margin-left: 2px;
      content: '';
      width: 16px;
      height: 16px;
      background-size: 16px 16px;
      transition: opacity 0.25s;
      background-image: url("data:image/svg+xml,%3Csvg xmlns='http://www.w3.org/2000/svg' width='24' height='24' viewBox='0 0 24 24'%3E%3Cpath d='M0 0h24v24H0z' fill='none'/%3E%3Cpath fill='%2307accb' d='M19 19H5V5h7V3H5c-1.11 0-2 .9-2 2v14c0 1.1.89 2 2 2h14c1.1 0 2-.9 2-2v-7h-2v7zM14 3v2h3.59l-9.83 9.83 1.41 1.41L19 6.41V10h2V3h-7z'/%3E%3C/svg%3E%0A");
      background-color: #fff;
      padding: 0px;
    }
    &:hover {
      &:after {
        opacity: 1;
      }
    }
  }
  @media print {
    text-decoration: none;
    color: #333333;
    text-underline: none;
    &.non-cta {
      font-style: italic;
      border: none;
    }
    &[target="_blank"]:after {
      display: none;
    }
  }
}

a.intro-link {
  color: #333333;
  text-decoration: underline;
  &:hover {
    color: lighten(#333333, 10);
    text-decoration: underline;
  }
  @media print {
    text-decoration: none;
  }
}

#app {
  margin: 0 auto;
  max-width: 1120px;
}

.fullpage {
  margin: 0 auto;
  max-width: 1120px;
}

.fullpage {
  position: relative;
  top: 0;
  right: 0;
  left: 0;
  bottom: 0;
  background: $bg;
  .overlay {
    position: fixed;
    top: 0;
    right: 0;
    left: 0;
    bottom: 0;
    background: rgba(#fff, 0.85);
    z-index: 2;
    pointer-events: none;
    opacity: 0;
    transition: opacity 0.15s cubic-bezier(1, 0, 0, 1);
  }
  &.is-contained {
    position: fixed;
    .overlay {
      display: block;
      pointer-events: auto;
      opacity: 1;
      transition: opacity 1.25s cubic-bezier(1, 0, 0, 1);
    }
  }
}

.hide-me {
  display: none;
}

.block-style {
  background: #FFFFFF;
  border-radius: $border-radius;
}

.block {
  h2 {
    transition: all 0.15s;
    margin-bottom: 16px;
  }
  hr {
    border-color: #DDDDDD;
    margin-top: 24px;
    margin-bottom: 24px;
  }
  .entry-row {
    display: flex;
    .entry {
      flex: 1;
      p {
        margin-bottom: 8px;
      }
    }
    &:last-child {
      .entry {
        p {
          margin-bottom: 0;
        }
      }
    }
  }
  .image-slide {
    height: 0px;
    overflow: hidden;
    transition: all 1s;
    white-space: nowrap;
    margin: -6px -24px;
    border-radius: 16px 16px 0 0;
    width: calc(100% + 48px);
    img {
      height: $image-slide-height;
      width: auto;
      margin-left: 1px;
      margin-right: 1px;
    }
  }
  .entry {
    span {
      &.year-inline {
        font-weight: 700;
        margin-right: 12px;
        color: #555555;
      }
      &.label-inline {
        display: inline-block;
        margin-right: 6px;
        // width: 72px;
      }
    }
    .title {
      h3, h4, h5, h6 {
        margin: 0;
        margin-bottom: 4px;
      }
      h4 {
        font-weight: 500;
        color: #333333;
        &.bold {
          font-weight: 600;
        }
      }
      h5 {
        font-weight: 500;
        color: #666666;
      }
      h6 {
        font-weight: 400;
        color: #888888;
      }
      padding-bottom: 2px;
      &.single-line {
        padding-bottom: 0px;
        h4 {
          font-weight: 600;
          color: #222222;
        }
      }
    }
    p, ul {
      margin-top: 4px;
      margin-bottom: 12px;
    }
    ul {
      padding-left: 20px;
      li {
        margin-top: 4px;
        margin-bottom: 6px;
      }
    }
    p {
      &.small {
        font-size: 13px;
        margin-top: 2px;
        margin-bottom: 10px;
      }
    }
    &:last-child {
      p:last-child {
        margin-bottom: 0;
      }
    }
  }
}

.btn {
  height: 42px;
  padding: 0 18px;
  border-radius: $border-radius;
  background: #FFFFFF;
  border: 1px solid #222222;
  font-weight: 500;
  margin-top: -4px;
  margin-bottom: 6px;
  transition: all 0.25s, color 0.1s;
  cursor: pointer;
  outline: 0;
  &:hover {
    background: $bg;
    color: #FFFFFF;
    border-color: darken($bg, 10);
    box-shadow: 0 0 4px 0 rgba(#000000, 0.1);
  }
  &.is-inline {
    height: 28px;
    padding: 0;
    border: none;
    text-decoration: underline;
    color: darken($bg, 15);
    transition: color 0.25s;
    &:hover {
      background: #FFFFFF;
      box-shadow: none;
      color: darken($bg, 10);
    }
  }
}

.only-print {
  display: none; // DEBUG-OFF
  // background: pink; // DEBUG-ON
  @media print {
    display: block;
  }
}

.only-interactive {
  display: block;
  // background: lightpink;
  @media print {
    display: none !important;
  }
}

@media print {
  h2 {
    color: darken($bg, 6);
  }
  body, html, .fullpage {
    background: #FFFFFF;
  }
  .block-style {
    border: 1px solid #DDDDDD;
  }
  .next-connect .block-style {
    border-bottom: none;
  }
  .is-connect .block-style {
    border-top: none;
    border-bottom: none;
  }
  .prev-connect .block-style {
    border-top: none;
  }
  .page-break {
    page-break-before: always;
  }
}
</style>
