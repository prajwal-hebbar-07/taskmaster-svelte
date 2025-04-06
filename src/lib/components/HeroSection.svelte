<script>
  import bookCover from "$assets/book_cover.png";
  import phoneCover from "$assets/phone_cover.png";
  import { Button } from "$components";
</script>

<section class="hero">
  <div class="hero-showcase text-center bold">
    <h1 class="purple">Move To</h1>
    <h1 class="purple mb-xs">Task Master</h1>
    <h4 class="italic">There is no need to struggle like I did.</h4>
    <img
      class="book-cover"
      src={bookCover}
      alt="Computer Screen for TaskMaster"
    />
    <img
      src={phoneCover}
      alt="Phone Screen for TaskMaster"
      class="phone-cover"
    />
  </div>
  <div class="hero-text bold white text-center">
    <h1>This Application</h1>
    <h1>Will Help You</h1>
    <h1>Save Your Time</h1>
    <h1 class="mb-m">And Efforts</h1>
    <p class="light-grey semi-bold italic mb-l">
      Lorem ipsum dolor sit amet, consectetur adipisicing elit. Ab iure dolorem
      accusantium tempora, consectetur modi non maiores! Corporis numquam ut
      iste fugit, quae temporibus reprehenderit recusandae dignissimos, iure
      totam expedita.
    </p>
    <Button>Get Premium for 10$/month</Button>
  </div>
</section>

<style>
  .hero {
    display: flex;
    height: 100vh;
    overflow-y: hidden;
  }

  .hero-showcase {
    position: relative;
    width: 50%;
    padding: 100px 16px 0 16px;
    background: linear-gradient(
      135deg,
      #e2cbff,
      #e2cbff 25%,
      #deeaff 50%,
      #ece5ff 75%,
      #927bce
    );
  }

  .hero-text {
    padding: 100px 5%;
    background-color: black;
    width: 50%;
  }

  .book-cover {
    position: absolute;
    right: 2%;
    bottom: 5%;
    width: 65%;
    /* transform: translateY(10%); */
  }

  .phone-cover {
    position: absolute;
    right: 60%;
    bottom: 20%;
    width: 30%;
  }
</style>
