---
layout: page
title: Auditions FAQs
---
<style>
  .faq-item {
    border-bottom: 1px solid #444;
    margin-bottom: 10px;
  }

  .faq-question {
    display: flex;
    justify-content: space-between;
    align-items: center;
    cursor: pointer;
    font-size: 18px;
    padding: 15px;
    background: #06001C;
    color: #F6F7FC;
    border: none;
    border-radius: 5px;
    transition: background 0.3s ease;
    font-weight: bold;
  }

  .faq-question:after {
    content: '+';
    font-size: 18px;
    color: #aaa;
    transition: transform 0.3s ease;
  }

  .faq-item.open .faq-question:after {
    content: '-';
    transform: rotate(180deg);
  }

  .faq-answer {
    max-height: 0;
    overflow: hidden;
    transition: opacity 0.3s ease, max-height 0.3s ease;
    font-size: 16px;
    background: #06001C;
    color: #F6F7FC;
    margin-top: 5px;
    padding: 0 15px;
    border-radius: 5px;
    opacity: 0;
  }

  .faq-item.open .faq-answer {
    max-height: 350px; 
    opacity: 1;
    padding: 10px 15px;
  }
</style>

<div class="faq-container">
  <div class="faq-item">
    <div class="faq-question" onclick="toggleFAQ(this)">When are auditions?</div>
    <div class="faq-answer">We generally hold auditions on the first or second weekend of both the Fall and Spring semesters. </div>
  </div>
  <div class="faq-item">
    <div class="faq-question" onclick="toggleFAQ(this)">Who can audition?</div>
    <div class="faq-answer">Any college student in the greater Boston area! We rarely take graduate students, but as long as you're enrolled in a degree program and are able to make it to rehearsals on Northeastern's campus you're welcome to try out.</div>
  </div>
  <div class="faq-item">
    <div class="faq-question" onclick="toggleFAQ(this)">What should I prepare for the audition?</div>
    <div class="faq-answer">
        We ask that you prepare a short solo between 60-90 seconds of a verse and a chorus from a song.
        Please try and pick a song that showcases your voice in the genre of music that we sing (pop, indie, etc.).<br><br>
        We ask that you do NOT sing any musical theater or opera pieces, or any other style very different from our style - check out our Spotify/YouTube to listen to our music!<br><br>

        In addition to your solo, we may ask you to do some vocal exercises, or potentially a second song, if we feel we don't yet have a good sense for your voice.
        If you are auditioning for VP, we ask you to prepare a set that showcases your entire kit.<br><br>

        We do NOT allow any background track or instruments to be played while you sing -- it must be completely a cappella!
    </div>
</div>
  <div class="faq-item">
    <div class="faq-question" onclick="toggleFAQ(this)">Do I need to sign up?</div>
    <div class="faq-answer">No, but it helps us out! We'll post signup links on our <a href="https://instagram.com/distilledharmonynu">Instagram</a> a few days before auditions, so you can make sure you get a slot at the time that suits you best. That being said, walk-ins are always welcome!</div>
  </div>
  <div class="faq-item">
    <div class="faq-question" onclick="toggleFAQ(this)">Is it hard to get in?</div>
    <div class="faq-answer">Our group usually has around 12-16 members, so auditions are definitely competitive, but we encourage everyone to audition! </div>
  </div>
  <div class="faq-item">
    <div class="faq-question" onclick="toggleFAQ(this)">Can I audition more than once?</div>
    <div class="faq-answer">Of course! The needs of the group are always changing, so you never know what we’re looking for in a particular semester. Many of our current group members didn't get in on their first try! </div>
</div>

<script>
  function toggleFAQ(element) {
    const parent = element.parentElement;
    parent.classList.toggle('open');
  }
</script>
