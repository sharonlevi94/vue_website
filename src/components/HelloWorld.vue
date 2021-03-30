<template>
  <v-container>
    <v-row class="text-center">
      <v-col cols="12">
        <v-img
          :src="require('../assets/sharon.png')"
          class="my-3"
          contain
          height="200"
        />
      </v-col>

      <v-col class="mb-4">
        <h1 class="display-2 font-weight-bold mb-3">
          ברוכים הבאים לאתר של שרון
        </h1>

        <p class="subheading font-weight-regular">
          Age: 27 | Live in Lapid | Computer Science Student
          <br>C | C++ | Python | HTML | CSS | JS | Assembly
          <br>
        </p>
      </v-col>

      <v-col
        class="mb-5"
        cols="12"
      >
        <h2 class="headline font-weight-bold mb-3">
          Contact me
        </h2>

        <v-row justify="center">
          <a
            v-for="(profile, i) in profilelists"
            :key="i"
            :href="profile.href"
            class="subheading mx-3"
            target="_blank"
          >
            <i :class="'fab fa-' +profile.text"></i>
          </a>
        </v-row>

        <v-row>
          <v-col class="mb-44">
            <h3 class="display-2 font-weight-bold mb-44">
              About
            </h3>
            <p>
              קוראים לי שרון לוי, בן 27, גר בלפיד. אני סטודנט שנה ב' למדעי המחשב במכללה האקדמית הדסה בירושלים<br>
              יש לי תשוקה רבה לתכנות! יש בי רצון ללמוד עוד, להתפתח ולהתקדם בעולם התכנות<br>
              בצבא הייתי קצין תותחנים ביחידה 611, הפעלתי מערכות מכ"ם מתקדמות ולחמתי במבצע צוק איתן <br>

            </p>

          </v-col>
        </v-row>

      </v-col>
    </v-row>
  </v-container>
</template>

<script>
  export default {
    name: 'HelloWorld',

    data: () => ({
      profilelists: [
        {
          text: 'facebook',
          href: 'https://www.facebook.com/sthth/',
        },
        {
          text: 'linkedin',
          href: 'https://www.linkedin.com/in/sharon-levy-8434471a5/',
        },
        {
          text: 'github',
          href: 'https://github.com/sharonlevi94',
        },
        {
          text: 'instagram',
          href: 'https://www.instagram.com/ssharonlevyy/',
        },
        {
          text: 'whatsapp',
          href: 'https://www.instagram.com/ssharonlevyy/',
        },
      ],

    }),
  }
</script>
