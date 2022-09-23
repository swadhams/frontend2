<script>
  import woman from "./assets/illustration-woman-online-desktop.svg";
  import pattern from "./assets/bg-pattern-desktop.svg";
  import arrow from "./assets/icon-arrow-down.svg";
  import box from "./assets/illustration-box-desktop.svg";
</script>

<main>
  <body>
    <div class="container">
      <div class="image">
        <!-- <img src={pattern} class="pattern" alt="" /> -->
        <img src={woman} class="woman" alt="Woman using a computer" />
        <!-- <img src={box} class="box" alt="A mailbox" /> -->
      </div>

      <div class="faq">
        <h2 class="h2">FAQ</h2>
        <div class="accordion">
          <details class="accordionItem">
            <summary class="accordionTitle">
              How many team members can I invite?
              <img src={arrow} alt="" class="arrowIcon" />
            </summary>
            <p>
              You can invite up to 2 additional users on the Free plan. There is
              no limit on team members for the Premium plan.
            </p>
          </details>
          <details class="accordionItem">
            <summary class="accordionTitle">
              What is the maximum file upload size?
              <img src={arrow} alt="" class="arrowIcon" />
            </summary>
            <p>
              No more than 2GB. All files in your account must fit your allotted
              storage space.
            </p>
          </details>
          <details class="accordionItem">
            <summary class="accordionTitle">
              How do I reset my password?
              <img src={arrow} alt="" class="arrowIcon" />
            </summary>
            <p>
              Click “Forgot password” from the login page or “Change password”
              from your profile page. A reset link will be emailed to you.
            </p>
          </details>
          <details class="accordionItem">
            <summary class="accordionTitle">
              Can I cancel my subscription?
              <img src={arrow} alt="" class="arrowIcon" />
            </summary>
            <p>
              Yes! Send us a message and we’ll process your request no questions
              asked.
            </p>
          </details>
          <details class="accordionItem">
            <summary class="accordionTitle">
              Do you provide additional support?
              <img src={arrow} alt="" class="arrowIcon" />
            </summary>
            <p>
              Chat and email support is available 24/7. Phone lines are open
              during normal business hours.
            </p>
          </details>
        </div>
      </div>
    </div>
  </body>
</main>

<style>
  
  .accordion {
    color: hsl(237, 12%, 33%);
  }
  .accordionItem {
    border-bottom: 1px solid hsl(240, 5%, 91%);
    padding: 1rem 0;  
  }
  .accordionItem[open] {
    font-weight: 700;
  }
  .accordionItem[open] .arrowIcon {
  transform: rotate(180deg);
  }
  .accordionTitle {
    cursor: pointer;
    list-style: none;
  }
  .accordionTitle:hover {
    color: orange;
  }
  body {
    width: 100%;
    max-width: 20rem;
    position: relative;
    border-radius: 1.5rem;
  }
  .container {
    border-radius: 1rem;
    background: white;
    display: grid;
    grid-template-columns: repeat(2, 1fr);
    max-height: 30rem;
    min-height: 30rem;
    overflow: scroll;
    position: relative;
  }
  .container::-webkit-scrollbar {
    display: none;
  }
  .faq {
    padding: 0 1.5rem;
    padding-bottom: 2.5rem;
    padding-top: 2.125rem;
  }
  .h2 {
    font-size: 2rem;
  }
  .image {
    position: relative;
    display: grid;
    justify-content: center;
    max-width: 100%;
    margin-top: 0;
    overflow: hidden;
    background-image: url("./assets/bg-pattern-desktop.svg");
    background-repeat: no-repeat;
    background-position: 50% 0;
  }
  main {
    align-content: center;
    background: linear-gradient(
      to bottom,
      hsl(273, 75%, 66%),
      hsl(240, 73%, 65%)
    );
    display: grid;
    font-family: "Kumbh Sans";
    justify-items: center;
    line-height: 1.5;
    min-height: 100vh;
  }
  p {
    font-size: 12px;
    font-weight: 400;
  }
  .woman{
  display: grid;
  height: 11rem;
  justify-content: center;
  width: 15rem;
  z-index: 2;
  }


  @media (min-width: 62em) {

}
  body {
    background-image: url("./assets/bg-pattern-desktop.svg");
    background-position: -35.5rem 65%;
    max-width: 57rem;
    position: relative;
  }
  body::before {
    content: url("./assets/illustration-box-desktop.svg");
    left: -10.5%;
    position: absolute;
    top: 39.5%;
    z-index: 3;
  } 
  .container {
    display: grid;
    grid-template-columns: repeat(2, 1fr);
    height: calc(512rem / 16);
    overflow: hidden;
    position: relative;
  }
  .image {
    margin-top: 0;
    overflow: hidden;
  }
  main {
    padding-top: 2rem;
  }
  .faq {
    padding-left: 2.25rem;
    padding-top: 3.25rem;
    padding-bottom: 5rem;
    padding-right: 4.75rem; 
    overflow-y: scroll;
    -ms-overflow-style: none;
    scrollbar-width: none; 
  }
  .faq::-webkit-scrollbar {
    display: none;
  }
.woman {
    height: 22rem;
    left: -9.5%;
    position: absolute;
    top: 14%;
    width: 30rem;
  }
</style>
