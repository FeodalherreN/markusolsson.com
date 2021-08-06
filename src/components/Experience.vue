<template>
  <div class="container text-center pb-5">
    <h2 class="header">Experience</h2>
    <div class="row">
      <div class="d-flex justify-content-center flex-nowrap">
        <Timeline
          :timeline-items="timelineItems"
          :message-when-no-items="messageWhenNoItems"
          class="pt-3"
        />
      </div>
    </div>
  </div>
</template>

<script>
import Timeline from "timeline-vuejs";
export default {
  name: "Experience",
  components: {
    Timeline,
  },
  data() {
    return {
      messageWhenNoItems: "No items found",
      timelineItems: [
        {
          from: new Date(2020, 5),
          title: "Developer at Telenor",
          description:
            "I am working with the website telenor.se with technologies as C#, Episerver, AWS (Elastic Beanstalk, Cloudwatch), ASP.NET, Docker and Vue.",
        },
        {
          from: new Date(2018, 9),
          title: "CTO and consultant at Digital Spark",
          description:
            "Me and a friend started this consultant company together, I was responsible for the technical parts of the projects we did inhouse, whilst also taking care of the employees and their knowledge development. I was consulting at Telenor at the same time.",
        },
        {
          from: new Date(2016, 10),
          title: "Consultant at XLENT",
          description:
            "Worked as a resource consultant for companies like Assembly, Kunskapsskolan, Interflora, Tunstall and Telenor. The technologies I used in these assigments was .NET, Java, Node.js, Episerver, Golang, Vue, AngularJS and SQL.",
        },
        {
          from: new Date(2016, 3),
          title: "Consultant at Axians",
          description:
            "Worked with web and API development for companies in need of improved IAM solutions. Forefront identity manager was the key in these projects, which is called Microsoft identity manager now a days. We synced all the identity data of the customers different systems (phone-system, active-directory, economy systems etc) and made sure everything as up to date and correct.",
        },
        {
          from: new Date(2015, 9),
          title: "Developer at Cloudfinder",
          description:
            "Cloudfinder was my first real job, I got the chance to meet amazing senior collegues that taught me the base of what I know today. We created an application that would enable version handling and searching of files in the cloud (Box, Office 365, Salesforce and Google). We used technologies as Java, C#, Docker, Elastic search and MongoDB.",
        },
        {
          from: new Date(2014, 6),
          title: "Trainee at CGI",
          description:
            "At CGI I was working as a trainee over the summer whilst still being in school. I got to work with internal salary systems that needed some care for. We added DevExpress and used their components to build a more modern UI for the time.",
        },
      ],
    };
  },
};
</script>