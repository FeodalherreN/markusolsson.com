<template>
  <section id="experience" class="section">
    <div class="container">
      <div class="surface experience">
        <div class="experience__head">
          <h2 class="header">Experience</h2>
          <div class="muted experience__hint">
            A quick timeline of where I’ve been building things.
          </div>
        </div>

        <div class="experience__timeline">
          <Timeline
            :timeline-items="timelineItems"
            :message-when-no-items="messageWhenNoItems"
          />
        </div>
      </div>
    </div>
  </section>
</template>

<script>
import Timeline from "timeline-vuejs";

export default {
  name: "Experience",
  components: { Timeline },
  data() {
    return {
      messageWhenNoItems: "No items found",
      timelineItems: [
        {
          from: new Date(2022, 1),
          title: "Developer at Softhouse",
          description:
            "Consultant at Softhouse, working as a solution architect at Skånetrafiken in Malmö. (C#, WPF, Azure, Kubernetes, Devops, Angular)",
        },
        {
          from: new Date(2020, 5),
          title: "Developer at Telenor",
          description:
            "Worked with telenor.se using C#, Episerver, AWS (Elastic Beanstalk, Cloudwatch), ASP.NET, Docker and Vue.",
        },
        {
          from: new Date(2018, 9),
          title: "CTO and consultant at Digital Spark",
          description:
            "Co-founded a consultant company. Responsible for technical delivery and knowledge development, while consulting at Telenor.",
        },
        {
          from: new Date(2016, 10),
          title: "Consultant at XLENT",
          description:
            "Resource consultant for Assembly, Kunskapsskolan, Interflora, Tunstall and Telenor. Tech: .NET, Java, Node.js, Episerver, Golang, Vue, AngularJS and SQL.",
        },
        {
          from: new Date(2016, 3),
          title: "Consultant at Axians",
          description:
            "Web/API development for IAM projects using Forefront Identity Manager (now Microsoft Identity Manager). Synced identity data across customer systems and kept everything consistent.",
        },
        {
          from: new Date(2015, 9),
          title: "Developer at Cloudfinder",
          description:
            "First real job — learned a ton from senior colleagues. Built a cloud file search/versioning product (Box, Office 365, Salesforce, Google). Tech: Java, C#, Docker, Elasticsearch and MongoDB.",
        },
        {
          from: new Date(2014, 6),
          title: "Trainee at CGI",
          description:
            "Summer trainee while in school. Modernized internal salary UIs using DevExpress components.",
        },
      ],
    };
  },
};
</script>

<style lang="scss" scoped>
.experience {
  padding: 22px;
}

.experience__head {
  padding: 8px 6px 0;
}

.experience__hint {
  margin-top: -6px;
  font-size: 14px;
}

.experience__timeline {
  margin-top: 18px;
  padding: 8px 0 6px;
}

/* timeline-vuejs overrides */
::v-deep .timeline-container {
  background: transparent;
}
::v-deep .timeline-item {
  border-radius: 14px;
  border: 1px solid rgba(255, 255, 255, 0.10);
  background: rgba(255, 255, 255, 0.05);
  box-shadow: 0 10px 28px rgba(0, 0, 0, 0.22);
}
::v-deep .timeline-item:hover {
  border-color: rgba(87, 226, 229, 0.22);
}
::v-deep .timeline-item-title {
  color: rgba(255, 255, 255, 0.92);
}
::v-deep .timeline-item-date {
  color: rgba(255, 255, 255, 0.58);
}
::v-deep .timeline-item-description {
  color: rgba(255, 255, 255, 0.72);
}
::v-deep .timeline-item-dot {
  background: linear-gradient(180deg, rgba(87, 226, 229, 1), rgba(253, 92, 99, 1));
  box-shadow: 0 0 0 5px rgba(87, 226, 229, 0.12);
}
</style>
