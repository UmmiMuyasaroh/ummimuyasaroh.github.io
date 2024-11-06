<script>
export default {
  data(){
    return {
      Project:[
        {
          year: " 2021 - Present",
          jobs: "Otomatisasi Makanan Kucing",
          company: "Universitas Amikom Yogyakarta",
          location: "Yogyakarta",
          description: [
            "The system is designed to automatically regulate feeding schedules, monitor cage temperature conditions and also monitor the amount of cat food. Users can manage schedules manually through the interface.",
          ]
        },
        {
          year: " 2022 - present",
          jobs: "Software Engineer",
          company: "Universitas Amikom Yogyakarta",
          location: "Yogyakarta",
          description: [
            "Developed numerous projects using Nuxt.js, harnessing its capabilities to create responsive and user-friendly front-end experiences.",
            "Played a pivotal role in establishing and implementing coding standards for Nuxt.js, ensuring consistency, readability, and maintainability across projects.",
            "Conducted code reviews, optimizations, and implemented best practices for scalable and maintainable codebases."
          ]
        },
        {
          year: "Sep 2021 - Nov 2021",
          jobs: "Intern Backend Developer",
          company: "Zerolim",
          location: "Remote",
          description: [
            "Gained hands-on experience in backend development tools such as Postman and GitLab, utilizing these tools to streamline development processes and enhance project workflows.",
            "Designed and developed APIs for internal Data Applications, contributing to the company's data management and accessibility initiatives.",
          ]
        }
      ]
    }
  }
}
</script>

<template>
  <section>
    <div class="d-flex align-items-center justify-content-between mb-4">
      <h2 class="text-primary fw-bolder mb-0">Experience</h2>
<!--      <a class="btn btn-primary px-4 py-3" href="#!">-->
<!--        <div class="d-inline-block bi bi-download me-2"></div>-->
<!--        Download Resume-->
<!--      </a>-->
    </div>

    <div v-for="experience of experiences" :key="'experience-index-' + experience.company" class="card shadow border-0 rounded-4 mb-5">
      <div class="card-body px-3 px-md-5 py-5">
        <div class="row align-items-center gx-5">
          <div class="col text-center text-lg-start mb-4 mb-lg-0">
            <div class="p-4 rounded-4">
              <div class="text-primary fw-bolder mb-2">{{experience.year}}</div>
              <div class="small fw-bolder">{{experience.jobs}}</div>
              <div class="small text-muted">{{experience.company}}</div>
              <div class="small text-muted">{{experience.location}}</div>
            </div>
          </div>
          <div class="col-lg-8">
            <div>
              <ul class="mb-0">
                <li v-for="desc of experience.description">
                  {{desc}}
                </li>
              </ul>
            </div>
          </div>
        </div>
      </div>
    </div>
  </section>
</template>

<style scoped>

</style>