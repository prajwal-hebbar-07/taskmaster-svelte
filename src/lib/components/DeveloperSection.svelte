<script>
  import ProfilePic from "$assets/profile_pic.png";
</script>

<section class="developer-section">
  <h2 class="mb-l">About the Developer</h2>
  <div class="developer-container">
    <div class="developer-text">
      <p class="mb-xs">
        Prajwal Hebbar A S is a skilled Frontend Web Application Developer with
        over three years of experience in designing and implementing responsive
        web designs. Specializing in technologies such as ReactJS, NextJS,
        Bootstrap, and MUI, Prajwal has a proven track record of thriving in
        fast-paced environments, particularly in startups where owning and
        managing complete projects is crucial. His expertise spans across
        various languages including JavaScript, TypeScript, HTML, CSS, and C,
        and he is adept at using UI libraries and CSS frameworks like MUI,
        Bootstrap 5, and TailwindCSS. Prajwal's professional journey includes
        significant roles at LYIK Technologies Private Limited, Content Enablers
        Inc., and Design Infuse, where he has led the development of
        client-facing applications, revamped company websites, and integrated
        analytics tools to enhance operational efficiency and SEO performance.
      </p>
      <p>
        In addition to his professional experience, Prajwal has contributed to
        notable projects such as "Quick Post" and "Culinary Community,"
        demonstrating his ability to work with a diverse tech stack including
        NodeJS and various frontend frameworks. He holds a Bachelor of
        Engineering in Computer Science from Vidyavardhaka College of
        Engineering, Mysuru, where he achieved a GPA of 8.50/10.00. Prajwal's
        language proficiency includes fluency in English, native-level Kannada,
        and proficiency in Hindi, making him a versatile and effective
        communicator in multilingual teams. His background and skills make him a
        valuable asset for any development team, particularly in roles that
        require a strong command of frontend technologies and a collaborative
        approach to project management.
      </p>
    </div>
    <img src={ProfilePic} alt="Prajwal Hebbar A S (Developer)" />
  </div>
</section>

<style>
  .developer-section {
    padding: 80px;
    margin-left: 12vw;
    margin-right: 12vw;
    max-width: 1280px;
  }

  .developer-container {
    display: flex;
    justify-content: space-between;
    align-items: center;
  }

  .developer-container img {
    width: 40%;
    height: 80%;
    border: 6px solid black;
    box-shadow: 0 4px 24px rgba(0, 0, 0, 0.5);
  }

  .developer-text {
    width: 54%;
  }
</style>
