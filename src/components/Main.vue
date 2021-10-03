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
            <div class="title mb-1">Socials</div>
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
            <div class="title mb-1">Hobbies</div>
            <v-divider></v-divider>
            <div class="text-center mt-3">
              <v-chip
                v-for="item in hobbies"
                :key="item.content"
                class="mr-2 mt-3"
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
                color="teal"
              >
                Listening
              </v-progress-circular>
              <v-progress-circular
                :rotate="360"
                :size="100"
                :width="6"
                value="80"
                color="teal"
                class="mx-10"
              >
                Reading
              </v-progress-circular>
              <v-progress-circular
                :rotate="360"
                :size="100"
                :width="6"
                value="60"
                color="teal"
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
              I'm a developer born in Nghe An, Vietnam
            </v-card-text>
            <v-card-text>
              I'm interested and skilled in different topics of Information
              Technology including programming, web development, and computer
              and network security
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
                  <strong>Good certificate of merit</strong>
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
                  <strong>Good certificate of merit</strong>
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
                  <v-col cols="12" md="6" v-for="item in skills" :key="item.title">
                    <div>
                      <v-avatar >
                        <v-icon>{{ item.icon }}</v-icon>
                      </v-avatar>
                      {{ item.title }}
                    </div>
                    <v-progress-linear
                      :color="item.color"
                      height="10"
                      value="10"
                      striped
                    ></v-progress-linear>
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
          value: "",
        },
        {
          icon: "mdi-vuejs",
          title: "VueJS Framework",
          color: "#42B883",
          value: "",
        },
        {
          icon: "mdi-language-javascript",
          title: "Javascript",
          color: "#f0db4f",
          value: "",
        },
        {
          icon: "mdi-language-html5",
          title: "HTML",
          color: "#e34c26",
          value: "",    
        },
        {
          icon: "mdi-language-css3",
          title: "CSS",
          color: "#2965f1",
          value: "",
        },
        {
          icon: "mdi-tailwind",
          title: "Tailwind CSS",
          color: "#26C6DA",
          value: "",
        },
         {
          icon: "mdi-vuetify",
          title: "Vuetify",
          color: "#039BE5",
          value: "",
        },
         {
          icon: "mdi-language-cpp",
          title: "C/C++/.NET",
          color: "#9575CD",
          value: "",
        },
         {
          icon: "mdi-bootstrap",
          title: "Bootstrap",
          color: "#563d7c",
          value: "",
        },  
      ],
      proud: [
        {
          icon: "mdi-help-rhombus-outline",
          title: "........................",
          subtitle: "....................",
        },
        {
          icon: "mdi-bookmark-music",
          title: "........................",
          subtitle: "....................",
        },
        {
          icon: "mdi-timer-sand",
          title: "........................",
          subtitle: "....................",
        },
        {
          icon: "mdi-account-multiple-outline",
          title: "........................",
          subtitle: "....................",
        },
      ],
      hobbies: [
        {
          icon: "mdi-bullseye",
          content: "Getting out of Safe Zone",
        },
        {
          icon: "mdi-biohazard",
          content: "Challenges",
        },
        {
          icon: "mdi-bike",
          content: "Cycling",
        },
        {
          icon: "mdi-image-filter-hdr",
          content: "Nature",
        },
        {
          icon: "mdi-music",
          content: "Music",
        },
        {
          icon: "mdi-gamepad-variant",
          content: "Games",
        },
        {
          icon: "mdi-airplane-takeoff",
          content: "Travel",
        },
        {
          icon: "mdi-book",
          content: "Book",
        },
        {
          icon: "mdi-account-group",
          content: "Leadership",
        },
        {
          icon: "mdi-bug",
          content: "Making bugs!",
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