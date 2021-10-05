<template>
  <Container name="contributor">
    <section class="content-section">
      <HashHeader title="CONTRIBUTORS" />
      <div class="contents">
        <div class="contributors-grid">
          <div
            v-for="(contributor, index) in contributors"
            :key="index"
            :class="[
              'contributor-card',
              `rot-${Math.floor(Math.random() * 24) * 15}`,
            ]"
          >
            <a
              :href="contributor.url"
              target="_blank"
              rel="noopener noreferrer"
            >
              <div class="picture-wrapper smooth-transition">
                <img
                  :src="contributor.picture"
                  alt="profile picture"
                  class="profile-pic"
                />
              </div>
            </a>
            <h4 class="title">{{ contributor.name }}</h4>
            <p v-if="contributor.description" class="description">
              {{ contributor.description }}
            </p>
          </div>
        </div>
      </div>
    </section>
  </Container>
</template>

<script>
import Container from "~/components/Container";
import HashHeader from "~/components/HashHeader";

export default {
  components: {
    Container,
    HashHeader,
  },
  data() {
    return {
      contributors: [
        {
          name: "Apoorv Dwivedi",
          url: "https://www.linkedin.com/in/apoorvdwi",
          picture: require("~/assets/Contributors/apoorv.jpeg"),
          description:
            "SWE Intern at Intervue | Microsoft Learn Student Ambassador | Core Team - HackOn 2.0, HackThisFall 2.0",
        },
        {
          name: "Manav Arora",
          url: "https://www.linkedin.com/in/manav-arora-0090b5202/",
          picture: require("~/assets/Contributors/Manav.jpg"),
          description:
            "Graphic Designer At Godwill Planners  | Flutter Developer | Game Developer | FreeLancer",
        },
        {
          name: "Aayush Kumar",
          url: "https://www.linkedin.com/in/aayushkum/",
          picture: require("~/assets/Contributors/aayush.jpg"),
          description:
            "Full Stack Developer | Ds-Algo | Android Lead at Google DSC NMIT",
        },
        {
          name: "Prateek Gupta",
          url: "https://linkedin.com/in/prateek-gupta-a600b6128",
          picture: require("~/assets/Contributors/Prateek.jpeg"),
          description: "Fullstack developer | cloud enthusiast | FreeLancer",
        },
        {
          name: "Vaibhav Jamwal",
          url: "https://www.linkedin.com/in/vaibhav-jamwal-4ba292194/",
          picture: require("~/assets/Contributors/despicabug.jpg"),
          description: "Web Developer",
        },
        {
          name: "Sudeep Deysarker",
          url: "https://www.linkedin.com/in/sudeep-deysarker",
          picture: require("~/assets/Contributors/lunaticsatoshi.jpg"),
          description:
            "Software Engineer | Full stack Developer | Android Developer | ML Enthusiast",
        },
        {
          name: "Alif Naufal Ilyas",
          url: "https://www.linkedin.com/in/alif-naufal-ilyas-b177a1207",
          picture: require("~/assets/Contributors/Natadesss.jpg"),
          description: "Student | DevOps Junior",
        },
        {
          name: "Anubhav",
          url: "https://www.linkedin.com/in/anubhavdev/",
          picture: require("~/assets/Contributors/anubhav.png"),
          description:
            "GWOC'21 Mentor | AngelHack Ambassdor | Open Source and Tech Enthusiast | ML Enthusiast",
        },
        {
          name: "Sahitya Roy",
          url: "https://www.linkedin.com/in/sahitya-roy/",
          picture: require("~/assets/Contributors/Sahitya.jpg"),
          description:
            "Co-Founder EduhubCommunity.tech| Building India's largest higher edtech community | Open Source enthusiast || Intern Geeksforgeeks || Keynote Speaker| Project Admin DevIncept | Youtuber || B.Tech CSE'24",
        },
        {
          name: "Manav Bansal",
          url: "https://www.linkedin.com/in/manavbansal11031998/",
          picture: require("~/assets/Contributors/Manav Bansal.jpg"),
          description:
            "Tech Enthusiast | Web Developer | Hackathons & Communities | Marketing | Ambassador | Traveler | Foodie",
        },
        {
          name: "Bhavesh Goyal",
          url: "https://www.linkedin.com/in/bhaveshgoyal182",
          picture: require("~/assets/Contributors/Bhaveshgoyal182.jpg"),
          description:
            "Junior | DevRel Enthusiast | Aspiring Full Stack Developer | Ex-Android Facilitator"
        },
        {
          name: "Narayan Soni",
          url: "https://www.linkedin.com/in/narayan-soni",
          picture: require("~/assets/Contributors/narayan_soni.png"),
          description: "Competitive coder | Freelancer | Open Source and Tech Enthusiast | ML Enthusiast"
        },
        {
          name: "Sriniketh J",
          url: "https://www.linkedin.com/in/sriniketh-jayasendil/",
          picture: require("~/assets/Contributors/Sriniketh.jpg"),
          description:
            "DS & ML Enthusiast | Learning WebDev | Sophomore at PSG iTech | GWOC- Contributor | HTF Evangelist | DS Intern @LGM @ TSF | Ninja Entrepreneur | CA@E-Cell, TechFest, MoodIndigo IIT-Bombay"
        },
        {
          name: "Ish Kapoor",
          url: "https://www.linkedin.com/in/ish-kapoor-2000ish/",
          picture: require("~/assets/Contributors/Ish.png"),
          description:
            "Robotics Engineer | Frontend Web Developer | GWOC- Contributor | AngelHack APAC Ambassador | HackClub Co-Lead"
        },
        {
          name: "Prakhar Sharma",
          url: "https://www.linkedin.com/in/prakhar-sharma-2206/",
          picture: require("~/assets/Contributors/Prakhar_Sharma.jpg"),
          description:
            "Computer Science Engineer | Full Stack Developer | DSC-MAIT Web Development lead "
        },
        {
          name: "Kushaggra Sharma",
          url: "https://www.linkedin.com/in/kushaggra-sharma/",
          picture: require("~/assets/Contributors/Kushaggra.jpeg"),
          description:
            "Software Engineer | Full Stack Developer | Open Source enthusiast "
        },
        {
          name: "Bhaskar Sharma",
          url: "https://www.linkedin.com/in/hoodooloo/",
          picture: require("~/assets/Contributors/bhaskar.jpg"),
          description:
            "Web Developer | Software Engineer | ML Enthusiast "
        },
        {
          name: "Mrunank Pawar",
          url: "https://www.linkedin.com/in/mrunankpawar/",
          picture: require("~/assets/Contributors/mrunank.PNG"),
          description:
            "Student | Google Crowdsource Influencer| Spark AR Campus Ambassador | AngelHack Student Ambassador | Hack Club Lead"
        },
        {
          name: "Kuwar Kapur",
          url: "https://www.linkedin.com/in/kuwar-kapur-936aa0183/",
          picture: require("~/assets/Contributors/kuwar.jpg"),
          description:
            "Robotics Engineer | Backend Developer | Machine Learning Developer | GSWOC contributor"
        },
        {
          name: "Sneha Sachdeva",
          url: "https://www.linkedin.com/in/sneha-sachdeva-5129501b0/",
          picture: require("~/assets/Contributors/Sneha.jpg"),
          description:
           "Student | Backend Intern at StartLadder| Tech Enthusiast"
        },
        {
          name: "Chirag Goel",
          url: "https://www.linkedin.com/in/chirag-goel-b578841b9/",
          picture: require("~/assets/Contributors/Chirag.jpg"),
          description:
            "Student | MERN Stack developer | GWOC- Contributor"
        },
        // Add you data here in the above format, don't change the existing order
      ],
    };
  },
};
</script>

<style lang="scss" scoped>
.content-section {
  display: flex;
  flex-direction: column;
  padding: 20px 0;
  font-family: "Segoe UI";
  margin: 2rem 0 1rem 0;

  .contents {
    padding: 1rem 4rem;
    text-align: center;

    @include respond-below(lg) {
      padding: 1rem 0rem;
    }

    .contributors-grid {
      display: grid;
      grid-template-columns: repeat(4, 1fr);
      column-gap: 20px;
      row-gap: 20px;

      @include respond-below(md) {
        grid-template-columns: repeat(3, 1fr);
      }

      @include respond-below(sm) {
        grid-template-columns: repeat(2, 1fr);
      }

      @include respond-below(xs) {
        grid-template-columns: repeat(1, 1fr);
      }

      .contributor-card {
        padding: 0.5rem 0 1rem;
        display: flex;
        flex-direction: column;
        box-shadow: rgba(255, 107, 0, 0.07) 0px 0px 10px 2px;
        border-radius: 1rem;
        // justify-content: center;
        align-items: center;

        .picture-wrapper {
          border-style: solid;
          border-width: 3px;
          border-color: red red white red;
          width: 210px;
          height: 210px;
          display: flex;
          align-items: center;
          justify-content: center;
          border-radius: 50%;
          margin-top: 1rem;

          .profile-pic {
            width: 200px;
            height: 200px;
            border-radius: 50%;
            // background: var(red);
          }

          @include respond-below(md) {
            width: 170px;
            height: 170px;
            .profile-pic {
              width: 160px;
              height: 160px;
            }
          }

          @include respond-below(sm) {
            width: 140px;
            height: 140px;
            .profile-pic {
              width: 130px;
              height: 130px;
            }
          }
        }

        .title {
          font-size: 1.2rem;
          text-align: center;
          margin: 1rem 0rem;
          color: rgba(233, 83, 34, 1);

          @include respond-below(sm) {
            font-size: 1rem;
            margin-top: 10px;
          }
        }

        .description {
          margin: 0 0.5rem 0.5rem;
          font-size: 1rem;
          color: #2b3531;
          line-height: 1.3rem;
          opacity: 0.7;
          text-align: center;
        }
      }
    }
  }
}
</style>
