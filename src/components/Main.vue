<template>
  <v-container>
    <v-row>
      <v-col cols="12" md="4">
        <v-card dark>
          <div class="text-center">
            <v-avatar class="mt-3" width="150" height="150">
              <v-img
                src="https://cdn.pixabay.com/photo/2015/04/23/22/00/tree-736885__480.jpg"
              >
              </v-img>
            </v-avatar>
          </div>

          <div class="text-center mt-3">
            <h1>Ho Sy Huy</h1>
            <span>A fresher front-end developer</span>
          </div>
          <v-container class="mt-3">
            <!-- Infomations -->
            <div class="title mb-1">INFO</div>
            <v-divider></v-divider>
            <v-list>
              <v-list-item v-for="item in info" :key="item.title">
                <v-list-item-avatar>
                  <v-icon>{{ item.icon }}</v-icon>
                </v-list-item-avatar>
                <v-list-item-content>
                  <v-list-item-title> {{ item.title }} </v-list-item-title>
                  <v-list-item-subtitle>
                    {{ item.content }}
                  </v-list-item-subtitle>
                </v-list-item-content>
              </v-list-item>
            </v-list>
            <!-- Social -->
            <div class="title mb-1">SOCIALS</div>
            <v-divider></v-divider>
            <v-list>
              <v-list-item v-for="item in socials" :key="item.title">
                <v-list-item-avatar>
                  <v-icon>{{ item.icon }}</v-icon>
                </v-list-item-avatar>
                <v-list-item-content>
                  <v-list-item-title>
                    <a
                      :href="item.content"
                      target="_blank"
                      style="text-decoration: none"
                      >{{ item.content }}</a
                    >
                  </v-list-item-title>
                </v-list-item-content>
              </v-list-item>
            </v-list>
            <!-- Hobbies -->
            <div class="title mb-1">HOBBIES</div>
            <v-divider></v-divider>
            <div class="text-center mt-3">
              <v-chip
                v-for="item in hobbies"
                :key="item.content"
                class="mr-2 mt-3"
                :color="item.color"
              >
                <v-avatar>
                  <v-icon>{{ item.icon }}</v-icon>
                </v-avatar>
                {{ item.content }}
              </v-chip>
            </div>
            <!-- Languages -->
            <div class="title mb-1">Languages</div>
            <v-divider></v-divider>
            <div class="text-center my-3 title">English</div>
            <div class="text-center">
              <v-progress-circular
                :rotate="360"
                :size="100"
                :width="6"
                value="70"
                color="#FFEBEE"
              >
                Listening
              </v-progress-circular>
              <v-progress-circular
                :rotate="360"
                :size="100"
                :width="6"
                value="80"
                color="#FFEBEE"
                class="mx-10"
              >
                Reading
              </v-progress-circular>
              <v-progress-circular
                :rotate="360"
                :size="100"
                :width="6"
                value="60"
                color="#FFEBEE"
              >
                Speaking
              </v-progress-circular>
            </div>
          </v-container>
        </v-card>
      </v-col>

      <v-col cols="12" md="8">
        <v-card>
          <v-container>
            <!-- introduce -->
            <v-card-title> Who am i ? </v-card-title>
            <v-divider></v-divider>
            <v-card-text>
              I'm a developer born in Nghe An, Vietnam. I'm a pretty introverted
              person
            </v-card-text>
            <v-card-text>
              Why did I choose IT? A question that is quite difficult for me to
              answer, well, I was born in a poor country, to be exposed to
              technology for me is quite a luxury. But everything changed when I
              moved south, and then I got to see for the first time this thing
              called a computer, which got me hooked, excited with all the
              wonderful things it had to offer. And from there my passion for
              computers grew. The older I get, the more I want to learn more
              about it, how it is made, how it works... .And now the passion for
              it is still burning inside of me.
            </v-card-text>
            <v-card-text>
              I'm interested and skilled in different topics of Information
              Technology including programming, web development, and computer
              and network security and I've always wanted to find a job related to something I'm passionate about
            </v-card-text>
            <!-- What am i proud of ? -->
            <v-card-title> What am i proud of ? </v-card-title>
            <v-divider></v-divider>
            <v-card-text>
              <v-list>
                <v-list-item v-for="item in proud" :key="item.title">
                  <v-list-item-avatar>
                    <v-icon>{{ item.icon }}</v-icon>
                  </v-list-item-avatar>
                  <v-list-item-content>
                    <v-list-item-title> {{ item.title }} </v-list-item-title>
                    <v-list-item-subtitle>
                      {{ item.subtitle }}
                    </v-list-item-subtitle>
                  </v-list-item-content>
                </v-list-item>
              </v-list>
            </v-card-text>
            <!-- Education -->
            <v-card-title> Education </v-card-title>
            <v-divider></v-divider>
            <v-card-text>
              <v-row>
                <v-col cols="12" md="4">2012 - 2016</v-col>
                <v-col cols="12" md="8">
                  <strong>Good certificate</strong>
                  <div>
                    <a
                      target="_blank"
                      href="http://ninhthuan.edu.vn/Default.aspx?sname=thptnguyendu&sid=1204&pageid=29310"
                      style="text-decoration: none"
                    >
                      Quang Trung Junior High School, Ninh Thuan</a
                    >
                  </div>
                </v-col>
              </v-row>
              <v-row>
                <v-col cols="12" md="4">2016 - 2018</v-col>
                <v-col cols="12" md="8">
                  <strong>Good certificate</strong>
                  <div>
                    <a
                      target="_blank"
                      href="http://ninhthuan.edu.vn/Default.aspx?sname=thptnguyendu&sid=1204&pageid=29310"
                      style="text-decoration: none"
                      >Nguyen Du High School, Ninh Thuan</a
                    >
                  </div>
                </v-col>
              </v-row>
              <v-row>
                <v-col cols="12" md="4">2018 - 2022 (not finished yet)</v-col>
                <v-col cols="12" md="8">
                  <strong>Engineering degree, Information Technology</strong>

                  <div>
                    <a
                      target="_blank"
                      href="http://ut.edu.vn/"
                      style="text-decoration: none"
                      >Ho Chi Minh City University of Transport</a
                    >
                  </div>
                  <div>
                    Became a member of University Academic Association of
                    Computer Science
                  </div>
                </v-col>
              </v-row>
            </v-card-text>
            <!-- Skill and Expertize -->
            <v-card flat>
              <v-card-title> Skill and Expertize </v-card-title>
              <v-divider></v-divider>
              <v-container>
                <v-row>
                  <v-col
                    cols="12"
                    md="6"
                    v-for="item in skills"
                    :key="item.title"
                  >
                    <div>
                      <v-avatar>
                        <v-icon>{{ item.icon }}</v-icon>
                      </v-avatar>
                      {{ item.title }}
                    </div>

                    <v-progress-linear
                      :color="item.color"
                      height="14"
                      :value="item.value"
                      rounded
                    >
                      <template v-slot:default="{ value }">
                        <strong>{{ Math.ceil(value) }}%</strong>
                      </template></v-progress-linear
                    >
                  </v-col>
                </v-row>
              </v-container>
            </v-card>
          </v-container>
        </v-card>
      </v-col>
    </v-row>
  </v-container>
</template>

<script>
export default {
  data() {
    return {
      skills: [
        {
          icon: "mdi-react",
          title: "React",
          color: "#61dbfb",
          value: "41",
        },
        {
          icon: "mdi-vuejs",
          title: "VueJS Framework",
          color: "#42B883",
          value: "73",
        },
        {
          icon: "mdi-language-javascript",
          title: "Javascript",
          color: "#FFD600",
          value: "71",
        },
        {
          icon: "mdi-language-html5",
          title: "HTML",
          color: "#e34c26",
          value: "62",
        },
        {
          icon: "mdi-language-css3",
          title: "CSS",
          color: "#2965f1",
          value: "42",
        },
        {
          icon: "mdi-tailwind",
          title: "Tailwind CSS",
          color: "#26C6DA",
          value: "27",
        },
        {
          icon: "mdi-vuetify",
          title: "Vuetify",
          color: "#039BE5",
          value: "66",
        },
        {
          icon: "mdi-bootstrap",
          title: "Bootstrap",
          color: "#563d7c",
          value: "17",
        },
      ],

      proud: [
        {
          icon: "mdi-trophy",
          title: "Achieve scholarships",
          subtitle: "Year 1, Year 2, Year 3",
        },
        {
          icon: "mdi-trophy-award",
          title: "Graduation ranking is excellent",
          subtitle: "In University",
        },
        {
          icon: "mdi-timer-sand",
          title: "The ability to schedule time",
          subtitle: "Know how to organize your time properly",
        },
        {
          icon: "mdi-account-multiple-outline",
          title: "Lead many groups and achieve high results",
          subtitle: "During university time ",
        },
      ],
      hobbies: [
        {
          icon: "mdi-bullseye",
          content: "Getting out of Safe Zone",
          color: "#E57373",
        },
        {
          icon: "mdi-biohazard",
          content: "Challenges",
          color: "#FF80AB",
        },
        {
          icon: "mdi-bike",
          content: "Cycling",
          color: "#CE93D8",
        },
        {
          icon: "mdi-image-filter-hdr",
          content: "Nature",
          color: "#2E7D32",
        },
        {
          icon: "mdi-music",
          content: "Music",
          color: "#B39DDB",
        },
        {
          icon: "mdi-gamepad-variant",
          content: "Games",
          color: "#80DEEA",
        },
        {
          icon: "mdi-airplane-takeoff",
          content: "Travel",
          color: "#26A69A",
        },
        {
          icon: "mdi-book",
          content: "Book",
          color: "#40C4FF",
        },
        {
          icon: "mdi-account-group",
          content: "Leadership",
          color: "#DCE775",
        },
        {
          icon: "mdi-bug",
          content: "Making bugs!",
          color: "#D7CCC8",
        },
      ],
      info: [
        {
          icon: "mdi-email",
          title: "Email",
          content: "syhuy851@gmail.com",
        },
        {
          icon: "mdi-earth",
          title: "My website",
          content: "hohuy.com",
        },
        {
          icon: "mdi-cake-layered",
          title: "Birthday",
          content: "Oct, 6, 2000",
        },
        {
          icon: "mdi-map-marker",
          title: "Habitation",
          content: "Ninh Thuan, Viet Nam",
        },
      ],
      socials: [
        {
          icon: "mdi-github",
          content: "https://github.com/hohuy852",
        },
        {
          icon: "mdi-linkedin",
          content: "https://www.linkedin.com/in/ho-sy-huy-0b2b8a192/",
        },
        {
          icon: "mdi-twitter",
          content: "https://twitter.com/Hohuy852",
        },
        {
          icon: "mdi-facebook",
          content: "https://www.facebook.com/hohuy852/",
        },
        {
          icon: "mdi-discord",
          content: "hohuy852#1914",
        },
        {
          icon: "mdi-reddit",
          content: "https://www.reddit.com/user/hohuy852",
        },
      ],
    };
  },
};
</script>

<style>
.v-tab {
  text-transform: none !important;
}
.theme--dark.v-sheet {
  background-color: #37474f !important;
  border-color: #1e1e1e;
  color: #ffffff;
}
.theme--light.v-sheet {
  background-color: #cfd8dc !important;
  border-color: #ffffff;
  color: rgba(0, 0, 0, 0.87);
}
</style>