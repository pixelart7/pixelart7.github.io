<template lang="pug">
.home
  PIntro
  .block-row
    .blocks
      .block.next-connect(ref="techskill"): PBlock
        .inner.block-style
          h2.expanded-title Technical Skills
          .entry
            .title.single-line
              h4 Programming Languages
            p JavaScript (ES7) and TypeScript, CSS (SCSS), Pug, HTML5, PHP
          .entry
            .title.single-line
              h4 Libraries, Frameworks and Tools
            p Vue 3, TailwindCSS, PWA, Firebase, Sketch, Laravel
          .only-expanded: hr
          .entry.only-expanded
            ul
             li: .
              Experienced a lot of working in a group environment
              both as a leader and a member.
              Can work in a global team and group using the English language.
             li: .
              Intermediate in website development, including developing,
              designing, testing, and deploying.
             li: .
              Highly experienced with modern website technology: HTML5,
              Javascript (ES6), CSS3, Bootstrap 4 CSS Framework,
              Bulma CSS Framework, Vue.
             li: .
              Experienced in developing a web application for offline usage
              with Google’s progressive web application specifications.
              Also with Firebase, contacting with various kind of APIs,
              such as Facebook API.
             li: .
              Can comfortably work in Node.js environment with various modules,
              such as Webpack, Vue, Babel, etc.
             li: .
              Highly experienced in managing servers, game servers,
              and social network pages.
             li: .
              Beginner in working with the internet of things and
              microprocessor environment.
          .only-interactive.only-collapsed
            button.btn.is-inline(@click="launchBlock('techskill')") Read more
      .block.prev-connect: PBlock
        .inner.block-style
          h2 Soft Skills
          .entry-row
            .entry: p Problem Solving
            .entry: p Data Collection & Analysis
          .entry-row
            .entry: p Communication
            .entry: p Teamwork
          .entry-row
            .entry: p Presentation
            .entry: p Public Speaking
      .block: PBlock
        .inner.block-style
          h2 Work Experiences
          .entry
            .title
              h3 Senior Solution Developer (Full-time, Remote)
              h4 Idea Vivat
              h5 10/2019 - Present
            p: .
              I work from a requirement gathering phase until the delivery of the solution.
              I am involved in both designing phase and developing phase.
          .entry
            .title
              h3 Freelance Web Solution Developer
              h5 Availability varies
            p: .
              Trusted by many agencies and companies, I work in my free-time.
              The scope of work that I usually involved with is in the front-end web development
              and technical project requirement gathering & planning.
            p: .
              Some of the final result that I worked before:
              a single-page app, an landing page, an interactive microsite for a short campaign,
              and an interactive web for digital signage.
          .entry
            .title
              h3 Game Server Administrator (Self-employed)
              h4 Siam Minecraft
              h5 2012 - 2015
            p: .
              Experienced in non-profit Minecraft game server administration.
              Built the web application used by players and staff team.
          hr(style="opacity: 0.25;")
          h3 Short-term
          .entry
            .title
              h4.bold Front-end Web Developer (Freelancer)
              h5 Idea Vivat
              h6 2016 - 2017, 04/2019 - 09/2019
            p.small: .
              Work project-based as part of the team at Idea Vivat.
              I involved in projects, such as POS system and money borrowing/lending system.
          .entry
            .title
              h4.bold Front-end Web Developer (Contract)
              h5 Muse Creative
              h6 10/2018 - Present
            p.small: .
              Designed and developed a web application for Muse Creative Portfolio
              design service. Worked with students from different universities.
          .entry
            .title
              h4.bold Product Management Trainee (Contract)
              h5 Digital Marketing at G-Able
              h6 09/2018 - 01/2019
            p.small: .
              Collaborate in a team environment in order to deliver an application
              and a solution as the client needs.
          .entry
            .title
              h4.bold Research Internship
              h5 Shibaura Institute of Technology
              h6 01/2018 - 03/2018
            p.small: .
              Worked with Prof. Hiroyuki Nakamura in the informal research
              about accessibility between Thailand and Japan.
      .block.next-connect.page-break: PBlock
        .inner.block-style
          h2 Side Projects
      .block.is-connect(ref="proj@to"): PBlock
        .inner.block-style
          .image-slide
            img(src="https://res.cloudinary.com/djtg2hopi/image/upload/v1605933295/portfolio/to-1.jpg")
          .entry
            .title
              h3.expanded-title To. Link Shortener
              h4
                span.label-inline Live:
                a.non-cta(@click="$event.stopPropagation();" href="https://to-url-shortener.netlify.app/" target="_blank") to-url-shortener.netlify.app
              h4
                span.label-inline Source:
                a.non-cta(@click="$event.stopPropagation();" href="https://github.com/pixelart7/to-link-shortener-web" target="_blank") github.com/pixelart7/to-link-shortener-web
                | ,
                |
                a.non-cta(@click="$event.stopPropagation();" href="https://github.com/pixelart7/to-link-shortener-surge-sh" target="_blank") /to-link-shortener-surge-sh
              h5 2019
            p: .
              An educational link shortener service that I built in order to learn AMP framework.
            .only-interactive.only-collapsed
              button.btn.is-inline(@click="launchBlock('proj@to')") View images
      .block.is-connect(ref="proj@gimme"): PBlock
        .inner.block-style
          .image-slide
            img(src="https://res.cloudinary.com/djtg2hopi/image/upload/v1605932852/portfolio/gimme-1.jpg")
            img(src="https://res.cloudinary.com/djtg2hopi/image/upload/v1605932845/portfolio/gimme-2.jpg")
            img(src="https://res.cloudinary.com/djtg2hopi/image/upload/v1605933118/portfolio/gimme-3.jpg")
          .entry
            .title
              h3.expanded-title Gimme Money
              h4
                span.label-inline Live:
                a.non-cta(@click="$event.stopPropagation();" href="https://gimme.netlify.app" target="_blank") gimme.netlify.app
              h4
                span.label-inline Source:
                a.non-cta(@click="$event.stopPropagation();" href="https://github.com/pixelart7/gimme-money" target="_blank") github.com/pixelart7/gimme-money
              h5 2019
            p: .
              Designed and built a simple application built on Vue with PWA for
              generating a PromptPay QR code with the desired amount of money.
            .only-interactive.only-collapsed
              button.btn.is-inline(@click="launchBlock('proj@gimme')") View images
      .block.is-connect(ref="proj@lyrics-base"): PBlock
        .inner.block-style
          .image-slide
            img(src="https://res.cloudinary.com/djtg2hopi/image/upload/v1548011506/portfolio/lyrics-1.jpg")
            img(src="https://res.cloudinary.com/djtg2hopi/image/upload/v1548011506/portfolio/lyrics-2.jpg")
          .entry
            .title
              h3.expanded-title Lyrics Base
              h4
                span.label-inline Live:
                a.non-cta(@click="$event.stopPropagation();" href="http://lyricsbase.pix7.me" target="_blank") lyricsbase.pix7.me
              h4
                span.label-inline Source:
                a.non-cta(@click="$event.stopPropagation();" href="http://github.com/pixelart7/lyrics-base-2" target="_blank") github.com/pixelart7/lyrics-base-2
              h5 2018
            p: .
              Designed and developed a web-based application on Vue with PWA
              for storing lyrics in two languages. The app is built with
              LocalStorage.js where all data are stored on the user's Google Drive.
            .only-interactive.only-collapsed
              button.btn.is-inline(@click="launchBlock('proj@lyrics-base')") View images
      .block.prev-connect(ref="proj@hon-no-jisho"): PBlock
        .inner.block-style
          .image-slide
            img(src="https://res.cloudinary.com/djtg2hopi/image/upload/v1548011506/portfolio/hon-1.jpg")
            img(src="https://res.cloudinary.com/djtg2hopi/image/upload/v1548011506/portfolio/hon-2.jpg")
          .entry
            .title
              h3.expanded-title Hon no Jisho
              h4
                span.label-inline Live:
                a.non-cta(@click="$event.stopPropagation();" href="https://hon-no-jisho.firebaseapp.com" target="_blank") hon-no-jisho.firebaseapp.com
              //- h4
                span.label-inline Source:
                a.non-cta(@click="$event.stopPropagation();" href="https://github.com/pixelart7/hon-no-jisho-2" target="_blank") github.com/pixelart7/hon-no-jisho-2
              h5 2018
            p: .
              Designed and developed a web-based application on Vue with PWA
              for storing book vocabulary in Japanese and English. Words are separated
              by section and chapters with an additional API calls to Japanese-English dictionary.
            .only-interactive.only-collapsed
              button.btn.is-inline(@click="launchBlock('proj@hon-no-jisho')") View images
    .blocks
      .block: PBlock
        .inner.block-style
          h2 Education
          .entry
            .title
              h3 B.Sc. Computer Science
              h4 King Mongkut’s University of Technology Thonburi
              h4 Bangkok, Thailand
              h5
                | 07/2015 - 11/2019
                br
                | Cumulative GPA: 3.80
            ul
              li
                span.year-inline 2019
                | Volunteer as a registrar in the event called
                |
                a.non-cta(href="https://www.eventpop.me/e/5651-azure-summer-spark", target="_blank") Azure Summer Spark
                |  held by KMUTT Microsoft Student Partner
              li
                span.year-inline 2019
                | Co-lead a seminar event on "
                a.non-cta(href="https://www.eventpop.me/e/5244-election-2019-the-future-of-science-and-technology", target="_blank") Thailand Election 2019: The Future of Thai Science and Technology
                | "
              li
                span.year-inline 2017 - 2018
                | One year study exchange to
                |
                a.non-cta(href="https://www.shibaura-it.ac.jp/en/", target="_blank") Shibaura Institute of Technology
                |  in Tokyo, Japan.
              li
                span.year-inline 2016 - 2017
                | Volunteer as the working group of KMUTT Cartoon Club.
              li
                span.year-inline 2016 - 2017
                | Participate in gPBL program twice, one in Japan and one in Thailand.
              li
                span.year-inline 2016
                .
                  Participate in international affair department as
                  buddies to assist foreign students.
              li
                span.year-inline 2015 - 2017
                | Lead the developer team of 2B-KMUTT camp to create an in-camp registrar program.
      .block: PBlock
        .inner.block-style
          h2 Languages
          .entry-row
            .entry
              .title
                h3 Thai
                h4 Native
            .entry
              .title
                h3 English
                h4 Fluent
                h5 TOEIC Test Score: 985/990
          .entry
            .title
              h3 Japanese
              h4 Basic
              h5 JLPT Test Level: N4
      .block: PBlock
        .inner.block-style
          h2 Interests
          .entry-row
            .entry: p Front-end Development
            .entry: p UI Design
          .entry-row
            .entry: p UX Design
            .entry: p Project Management
          .entry-row
            .entry: p Foreign Cultures
            .entry: p Traveling
</template>

<script>
import PIntro from '@/components/portfolio/Intro.vue';
import PBlock from '@/components/portfolio/Block.vue';

export default {
  data: () => ({
    isBlockExpanded: false,
    expandedBlockRef: '',
  }),
  mounted() {
    // console.log(this.$route.params)
    if (Object.hasOwnProperty.call(this.$route.params, 'pseudoPath')) {
      this.launchBlock(this.$route.params.pseudoPath);
    }
  },
  watch: {
    $route() {
      this.routeHandler();
    },
  },
  methods: {
    routeHandler() {
      if (this.isBlockExpanded && this.$route.name === 'home') {
        const blk = this.$refs[this.expandedBlockRef];
        const blkRect = blk.getBoundingClientRect();
        const fp = document.getElementById('fullpage');
        const fpRect = fp.getBoundingClientRect();
        const blkComponent = blk.querySelector('.block-component');
        // const blkComponentRect = blkComponent.getBoundingClientRect();
        const innerBlk = blkComponent.querySelector('.inner');
        if (window.innerWidth < 570) {
          blkComponent.style.cssText = `top: ${blkRect.top + (-fpRect.top)}px; right: 8px; left: 8px; bottom: ${blkRect.bottom}px;`;
        } else {
          blkComponent.style.cssText = `top: ${blkRect.top + (-fpRect.top)}px; right: ${blkRect.right - ((window.innerWidth - fpRect.width) / 2) + 8}px; left: ${blkRect.left - ((window.innerWidth - fpRect.width) / 2)}px; bottom: ${blkRect.bottom}px;`;
        }
        innerBlk.style.cssText = `height: ${blkRect.height}px;`;
        blk.classList.add('is-contracting');
        setTimeout(() => {
          blk.classList.remove('is-expanded');
          const topOffset = parseFloat(fp.style.cssText.replace(/[^\d\.]/g,'')); // eslint-disable-line
          fp.classList.remove('is-contained');
          blk.classList.remove('is-contracting');
          fp.style.cssText = '';
          blkComponent.style.cssText = '';
          innerBlk.style.cssText = '';
          blk.style.cssText = '';
          window.scrollTo({ top: topOffset });
        }, 1000);
        this.isBlockExpanded = false;
      }
    },
    launchBlock(e) {
      if (this.isBlockExpanded) return;
      this.$router.push({ name: 'homeExpanded', params: { pseudoPath: e } });
      this.expandedBlockRef = e;
      const blk = this.$refs[e];
      const blkRect = blk.getBoundingClientRect();
      const fp = document.getElementById('fullpage');
      const fpRect = fp.getBoundingClientRect();
      const blkComponent = blk.querySelector('.block-component');
      const blkComponentRect = blkComponent.getBoundingClientRect();
      const innerBlk = blkComponent.querySelector('.inner');
      fp.style.cssText = `top: ${fpRect.top - 8}px`;
      fp.classList.add('is-contained');
      blk.style.cssText = `height: ${blkRect.height}px; width: ${blkRect.width}px; background: #FFFFFF`;
      if (window.innerWidth < 570) {
        blkComponent.style.cssText = `top: ${blkComponentRect.top + (-fpRect.top)}px; right: 8px; left: 8px; bottom: ${blkComponentRect.bottom}px;`;
      } else {
        blkComponent.style.cssText = `top: ${blkComponentRect.top + (-fpRect.top)}px; right: ${blkComponentRect.right - ((window.innerWidth - fpRect.width) / 2) + 8}px; left: ${blkComponentRect.left - ((window.innerWidth - fpRect.width) / 2)}px; bottom: ${blkComponentRect.bottom}px;`;
      }
      innerBlk.style.cssText = `height: ${innerBlk.getBoundingClientRect().height}px;`;
      blk.classList.add('is-expanded');
      setTimeout(() => { blkComponent.style.cssText = `top: ${(-fpRect.top + 8 + 8)}px;`; }, 0);
      setTimeout(() => { innerBlk.style.cssText = ''; }, 250);
      this.isBlockExpanded = true;
    },
  },
  components: { PIntro, PBlock },
};
</script>

<style lang="scss">
$image-slide-height: 360px;

.home {
  $common-margin: 8px;
  .block-row {
    display: flex;
    padding: $common-margin / 2;
    .blocks {
      flex: 1;
      max-width: 50%;
      .block {
        margin: $common-margin / 2;
        margin-bottom: $common-margin;
        &.is-connect {
          margin-top: 0;
          margin-bottom: 0;
          .inner {
            border-radius: 0;
            padding-top: 6px;
            padding-bottom: 12px;
          }
        }
        &.next-connect {
          margin-bottom: 0;
          .inner {
            border-bottom-left-radius: 0;
            border-bottom-right-radius: 0;
            padding-bottom: 2px;
          }
        }
        &.prev-connect:not(.is-expanded) {
          margin-top: 0;
          .inner {
            border-top-left-radius: 0;
            border-top-right-radius: 0;
            padding-top: 6px;
            h2 {
              margin-top: 12px;
            }
          }
        }
        .only-collapsed, .only-expanded {
          transition: all 1s cubic-bezier(1, 0, 0, 1);
        }
        .only-expanded {
          overflow-y: hidden;
          opacity: 0;
          height: 0px;
        }
        &.is-expanded {
          .image-slide {
            transition: all 0.5s cubic-bezier(1, 0, 0, 1);
            transition-delay: 0.65s;
            height: $image-slide-height;
            overflow-x: scroll;
            white-space: nowrap;
            border-bottom: 1px solid #EEEEEE;
          }
          .block-component {
            position: absolute;
            z-index: 3;
            top: 0px;
            right: 8px;
            left: 8px;
            bottom: 8px;
            margin: 48px 128px;
            .inner {
              height: 100%;
              overflow-y: scroll;
              box-shadow: 0px 0px 64px 1px rgba(0,0,0,0.2), 0px 6px 12px 1px rgba(0,0,0,0.15);
              border-radius: 16px;
            }
            @media only screen and (max-width: 768px) {
              margin: 48px;
            }
            @media only screen and (max-width: 570px) {
              margin: 8px;
              margin-bottom: 64px;
            }
          }
          .expanded-title {
            font-size: 28px;
            transition: all 0.35s;
            margin-top: 32px;
            margin-bottom: 18px;
            // transform: scale(2);
            // transform-origin: 0 0;
          }
          .only-collapsed {
            overflow-y: hidden;
            height: 0px;
            opacity: 0;
          }
          .only-expanded {
            overflow-y: visible;
            opacity: 1;
            height: auto;
          }
        }
        &.is-contracting {
          .image-slide {
            height: 0px;
            overflow-x: scroll;
            transition: all 0.75s cubic-bezier(1, 0, 0, 1);
            transition-delay: 0s;
          }
          .only-collapsed {
            overflow-y: hidden;
            height: 0px;
            opacity: 0;
          }
          .expanded-title {
            font-size: 24px;
            margin-top: 6px;
            margin-bottom: 6px;
          }
          .block-component {
            margin: 0px;
            .inner {
              border-radius: 0px;
              transform: scale(1.01);
              transition: all 1s, transform 0.1s;
              // box-shadow: 0px 6px 6px 1px rgba(0,0,0,0.15);
            }
          }
          .only-expanded {
            overflow-y: hidden;
            opacity: 0;
          }
        }
      }
      &:first-child {
        .block {
          margin-right: $common-margin / 2;
        }
      }
      &:last-child {
        .block {
          margin-left: $common-margin / 2;
        }
      }
    }
    @media only screen and (max-width: 570px) {
      flex-direction: column-reverse;
      .blocks {
        max-width: initial;
      }
    }
  }
}
</style>
