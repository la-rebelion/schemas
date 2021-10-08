# Schema



## YAML Example

```yaml
@startyaml{.plantuml caption="Events Schema"}
name: We Are Developers 2024
slug: we-are-developers-2024
featured: true
shortname: DevConf 2024 # i.e. You can define the marketing name of the event or the vendor name
date: 2024-10-17 10:00:00 -0500
end-date: 2024-10-19 18:00:00 -0500
picture: https://images.unsplash.com/photo-1503428593586-e225b39bddfe?ixlib=rb-1.2.1&ixid=MnwxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8&auto=format&fit=crop&w=320&q=80
location: New York, USA
# Accepts markdown and HTML
heading: "This a featured event, you can modify `_data` file to change it."
# Each section can have its own CTA
# Main (hero) Call To Action
cta:
  link: https://rebelion.la/
  text: Get Tickets
about:
  cta:
    link: https://rebelion.la/
    text: Get Your Ticket Today
  # supports markdown and HTML
  description: >
    Briefly introduce your conference or event here. You should convince people 
    why they should attend with a list of benefits. **Are you a conference organizer? 
    Want to source rebelion t-shirts as part of your conference package?** Check 
    out our Rebelion tees at [rebelion.la](https://rebelion.la/coming-soon) - 
    developers love them! Want to get a bulk discount or just want to use one of 
    the t-shirt designs? Please email 
    <a href="mailto:viva@rebelion.la">viva@rebelion.la</a> and we can discuss.
  highlights:
    heading: Why Join Us
    highlights-list:
      - "**Unique chance** to lorem ipsum dolor"
      - Learn from the best in the industry
      - Discover the best tools and practices
      - Meet developers from all over the world
      - Grow your network
      - Practical workshops to lorem ipsum dolor
      - After-party lorem ipsum dolor
      - Free <a href="https://rebelion.la">t-shirts</a> and swag
stats:
  # Group is introduced to allow you to include more than one section with same format, different data ;)
  # Just be aware, group names CAN NOT be duplicated, only the first one found is used
  - group: attendees
    stats-details:
      - unit: Attendees
        number: 2000+
      - unit: Days
        number: 3
      - unit: Talks
        number: 60+
      - unit: Workshops
        number: 10+
speakers:
  intro: >
    List your featured speakers here. You can provide more info about each 
    speaker in the relevant modal windows. Lorem ipsum dolor sit amet, consectetur 
    adipiscing elit.
  cta:
    link: https://rebelion.la
    text: Get Tickets
  speaker:
    - name: James Escutia
      slug: james-escutia
      picture: assets/images/speakers/speaker-1.jpg
      role: Senior Software Developer
      organization: Angular Core Team
      # Supports HTML tags, but NO markdown :(
      summary: >
        <p>You can put speaker's bio or talk related info here. Duis a mi quis metus 
        porttitor eleifend. Pellentesque finibus ultrices imperdiet. Maecenas auctor 
        tortor quis risus tincidunt, mattis mattis leo placerat. Fusce metus augue, 
        sagittis eget enim vel, venenatis auctor est. In interdum felis massa, ac porta 
        nunc pretium non. In fringilla orci vitae imperdiet malesuada. Vestibulum feugiat 
        lobortis est, in sagittis nisi molestie vel. Mauris ultrices vitae lectus eu 
        feugiat. Fusce semper, nisi at placerat mollis, augue elit pretium enim, eu 
        pellentesque justo purus et lectus.</p>

        <p class="mb-0">Donec neque magna, molestie vel varius ut, pretium a urna. Pellentesque placerat 
        nunc eu condimentum pellentesque. Vivamus dictum nisl leo, id fermentum lectus 
        porttitor et. Pellentesque tristique erat libero, condimentum porttitor nisl 
        pharetra et.</p>
      github: adrianescutia
      linkedin: adrianescutia
      twitter: AdES_MX
    - name: Sarah Escutia
      slug: sarah-escutia
      picture: assets/images/speakers/speaker-2.jpg
      role: Developer Advocate
      organization: Google
      summary: >
        You can put speaker's bio or talk related info here. Duis a mi quis metus 
        porttitor eleifend. Pellentesque finibus ultrices imperdiet. Maecenas auctor 
        tortor quis risus tincidunt, mattis mattis leo placerat. Fusce metus augue, 
        sagittis eget enim vel, venenatis auctor est. In interdum felis massa, ac porta 
        nunc pretium non. In fringilla orci vitae imperdiet malesuada. Vestibulum feugiat 
        lobortis est, in sagittis nisi molestie vel. Mauris ultrices vitae lectus eu 
        feugiat. Fusce semper, nisi at placerat mollis, augue elit pretium enim, eu 
        pellentesque justo purus et lectus.

        Donec neque magna, molestie vel varius ut, pretium a urna. Pellentesque placerat 
        nunc eu condimentum pellentesque. Vivamus dictum nisl leo, id fermentum lectus 
        porttitor et. Pellentesque tristique erat libero, condimentum porttitor nisl 
        pharetra et.
      github: adrianescutia
      linkedin: adrianescutia
      twitter: AdES_MX
    - name: Tim Escutia
      slug: tim-escutia
      picture: assets/images/speakers/speaker-3.jpg
      role: Software Developer
      organization: React Core Team
      summary: >
        You can put speaker's bio or talk related info here. Duis a mi quis metus 
        porttitor eleifend. Pellentesque finibus ultrices imperdiet. Maecenas auctor 
        tortor quis risus tincidunt, mattis mattis leo placerat. Fusce metus augue, 
        sagittis eget enim vel, venenatis auctor est. In interdum felis massa, ac porta 
        nunc pretium non. In fringilla orci vitae imperdiet malesuada. Vestibulum feugiat 
        lobortis est, in sagittis nisi molestie vel. Mauris ultrices vitae lectus eu 
        feugiat. Fusce semper, nisi at placerat mollis, augue elit pretium enim, eu 
        pellentesque justo purus et lectus.

        Donec neque magna, molestie vel varius ut, pretium a urna. Pellentesque placerat 
        nunc eu condimentum pellentesque. Vivamus dictum nisl leo, id fermentum lectus 
        porttitor et. Pellentesque tristique erat libero, condimentum porttitor nisl 
        pharetra et.
      github: adrianescutia
      linkedin: adrianescutia
      twitter: AdES_MX
    - name: Josh Escutia
      slug: josh-escutia
      picture: assets/images/speakers/speaker-4.jpg
      role: Founder &amp; CTO
      organization: Startup Week
      summary: >
        You can put speaker's bio or talk related info here. Duis a mi quis metus 
        porttitor eleifend. Pellentesque finibus ultrices imperdiet. Maecenas auctor 
        tortor quis risus tincidunt, mattis mattis leo placerat. Fusce metus augue, 
        sagittis eget enim vel, venenatis auctor est. In interdum felis massa, ac porta 
        nunc pretium non. In fringilla orci vitae imperdiet malesuada. Vestibulum feugiat 
        lobortis est, in sagittis nisi molestie vel. Mauris ultrices vitae lectus eu 
        feugiat. Fusce semper, nisi at placerat mollis, augue elit pretium enim, eu 
        pellentesque justo purus et lectus.

        Donec neque magna, molestie vel varius ut, pretium a urna. Pellentesque placerat 
        nunc eu condimentum pellentesque. Vivamus dictum nisl leo, id fermentum lectus 
        porttitor et. Pellentesque tristique erat libero, condimentum porttitor nisl 
        pharetra et.
      github: adrianescutia
      linkedin: adrianescutia
      twitter: AdES_MX
    - name: Ling Escutia
      slug: ling-escutia
      picture: assets/images/speakers/speaker-5.jpg
      role: Software Architect
      organization: GitHub
      summary: >
        You can put speaker's bio or talk related info here. Duis a mi quis metus 
        porttitor eleifend. Pellentesque finibus ultrices imperdiet. Maecenas auctor 
        tortor quis risus tincidunt, mattis mattis leo placerat. Fusce metus augue, 
        sagittis eget enim vel, venenatis auctor est. In interdum felis massa, ac porta 
        nunc pretium non. In fringilla orci vitae imperdiet malesuada. Vestibulum feugiat 
        lobortis est, in sagittis nisi molestie vel. Mauris ultrices vitae lectus eu 
        feugiat. Fusce semper, nisi at placerat mollis, augue elit pretium enim, eu 
        pellentesque justo purus et lectus.

        Donec neque magna, molestie vel varius ut, pretium a urna. Pellentesque placerat 
        nunc eu condimentum pellentesque. Vivamus dictum nisl leo, id fermentum lectus 
        porttitor et. Pellentesque tristique erat libero, condimentum porttitor nisl 
        pharetra et.
      github: adrianescutia
      linkedin: adrianescutia
      twitter: AdES_MX
    - name: Andy Escutia
      slug: andy-escutia
      picture: assets/images/speakers/speaker-6.jpg
      role: Senior Software Engineer
      organization: Twitter
      summary: >
        You can put speaker's bio or talk related info here. Duis a mi quis metus 
        porttitor eleifend. Pellentesque finibus ultrices imperdiet. Maecenas auctor 
        tortor quis risus tincidunt, mattis mattis leo placerat. Fusce metus augue, 
        sagittis eget enim vel, venenatis auctor est. In interdum felis massa, ac porta 
        nunc pretium non. In fringilla orci vitae imperdiet malesuada. Vestibulum feugiat 
        lobortis est, in sagittis nisi molestie vel. Mauris ultrices vitae lectus eu 
        feugiat. Fusce semper, nisi at placerat mollis, augue elit pretium enim, eu 
        pellentesque justo purus et lectus.

        Donec neque magna, molestie vel varius ut, pretium a urna. Pellentesque placerat 
        nunc eu condimentum pellentesque. Vivamus dictum nisl leo, id fermentum lectus 
        porttitor et. Pellentesque tristique erat libero, condimentum porttitor nisl 
        pharetra et.
      github: adrianescutia
      linkedin: adrianescutia
      twitter: AdES_MX
    - name: Alice Escutia
      slug: alice-escutia
      picture: assets/images/speakers/speaker-7.jpg
      role: Senior Software Developer
      organization: Facebook
      summary: >
        You can put speaker's bio or talk related info here. Duis a mi quis metus 
        porttitor eleifend. Pellentesque finibus ultrices imperdiet. Maecenas auctor 
        tortor quis risus tincidunt, mattis mattis leo placerat. Fusce metus augue, 
        sagittis eget enim vel, venenatis auctor est. In interdum felis massa, ac porta 
        nunc pretium non. In fringilla orci vitae imperdiet malesuada. Vestibulum feugiat 
        lobortis est, in sagittis nisi molestie vel. Mauris ultrices vitae lectus eu 
        feugiat. Fusce semper, nisi at placerat mollis, augue elit pretium enim, eu 
        pellentesque justo purus et lectus.

        Donec neque magna, molestie vel varius ut, pretium a urna. Pellentesque placerat 
        nunc eu condimentum pellentesque. Vivamus dictum nisl leo, id fermentum lectus 
        porttitor et. Pellentesque tristique erat libero, condimentum porttitor nisl 
        pharetra et.
      github: adrianescutia
      linkedin: adrianescutia
      twitter: AdES_MX
    - name: Thomas Escutia
      slug: thomas-escutia
      picture: assets/images/speakers/speaker-8.jpg
      role: Lead Developer
      organization: Microsoft
      summary: >
        You can put speaker's bio or talk related info here. Duis a mi quis metus 
        porttitor eleifend. Pellentesque finibus ultrices imperdiet. Maecenas auctor 
        tortor quis risus tincidunt, mattis mattis leo placerat. Fusce metus augue, 
        sagittis eget enim vel, venenatis auctor est. In interdum felis massa, ac porta 
        nunc pretium non. In fringilla orci vitae imperdiet malesuada. Vestibulum feugiat 
        lobortis est, in sagittis nisi molestie vel. Mauris ultrices vitae lectus eu 
        feugiat. Fusce semper, nisi at placerat mollis, augue elit pretium enim, eu 
        pellentesque justo purus et lectus.

        Donec neque magna, molestie vel varius ut, pretium a urna. Pellentesque placerat 
        nunc eu condimentum pellentesque. Vivamus dictum nisl leo, id fermentum lectus 
        porttitor et. Pellentesque tristique erat libero, condimentum porttitor nisl 
        pharetra et.
      github: adrianescutia
      linkedin: adrianescutia
      twitter: AdES_MX
schedule:
  dates:
    - date: 2024-10-17 9:00:00 -0500
      heading: Day 1
      plan:
      - start-time: 9:00:00 -0500
        end-time: 9:30:00 -0500
        conference: Best Practices And Tips For A Clean Angular Application
        location: Conference Room A
        # Supports markdown and HTML, both! :)
        summary: >
          Talk's summary goes here. <b>You can hook up the speaker profile image/name 
          on the left with his or her bio modal window</b>. Lorem ipsum dolor sit amet, 
          consectetur adipiscing elit. Fusce quis ornare nibh, pulvinar posuere justo. 
          Aenean laoreet nunc a eleifend lacinia. Phasellus dignissim augue at 
          consectetur ullamcorper.
        speaker: james-escutia
      - start-time: 9:30:00 -0500
        end-time: 10:00:00 -0500
        conference: Developer Productivity
        location: Conference Room A
        summary: >
          Talk's summary goes here. **You can hook up the speaker profile image/name 
          on the left with his or her bio modal window**. Lorem ipsum dolor sit amet, 
          consectetur adipiscing elit. Fusce quis ornare nibh, pulvinar posuere justo. 
          Aenean laoreet nunc a eleifend lacinia. Phasellus dignissim augue at 
          consectetur ullamcorper.
        speaker: sarah-escutia
      - start-time: 10:00:00 -0500
        end-time: 10:30:00 -0500
        conference: Coffee Break
        location: Room A5
        summary: >
          Coffee and cakes lorem ipsum dolor sit amet, consectetur adipiscing elit.
      - start-time: 10:30:00 -0500
        end-time: 11:00:00 -0500
        conference: Progressive Web Apps with React.js
        location: Conference Room A
        summary: >
          Talk's summary goes here. **You can hook up the speaker profile image/name 
          on the left with his or her bio modal window**. Lorem ipsum dolor sit amet, 
          consectetur adipiscing elit. Fusce quis ornare nibh, pulvinar posuere justo. 
          Aenean laoreet nunc a eleifend lacinia. Phasellus dignissim augue at 
          consectetur ullamcorper.
        speaker: tim-escutia
      - start-time: 11:00:00 -0500
        end-time: 12:00:00 -0500
        conference: Talk Title Lorem Ipsum
        location: Conference Room B
        summary: >
          Talk's summary goes here. **You can hook up the speaker profile image/name 
          on the left with his or her bio modal window**. Lorem ipsum dolor sit amet, 
          consectetur adipiscing elit. Fusce quis ornare nibh, pulvinar posuere justo. 
          Aenean laoreet nunc a eleifend lacinia. Phasellus dignissim augue at 
          consectetur ullamcorper.
        speaker: josh-escutia
      - start-time: 12:00:00 -0500
        end-time: 13:30:00 -0500
        conference: Lunch Break
        location: Room B6
        summary: >
          Buffet lorem ipsum dolor sit amet, consectetur adipiscing elit.
        #speaker: the-chef
      - start-time: 13:30:00 -0500
        end-time: 14:30:00 -0500
        conference: Talk Title Lorem Ipsum
        location: Conference Room A
        summary: >
          Talk's summary goes here. **You can hook up the speaker profile image/name 
          on the left with his or her bio modal window**. Lorem ipsum dolor sit amet, 
          consectetur adipiscing elit. Fusce quis ornare nibh, pulvinar posuere justo. 
          Aenean laoreet nunc a eleifend lacinia. Phasellus dignissim augue at 
          consectetur ullamcorper.
        speaker: ling-escutia
      - start-time: 14:30:00 -0500
        end-time: 15:30:00 -0500
        conference: Talk Title Lorem Ipsum
        location: Conference Room C
        summary: >
          Talk's summary goes here. **You can hook up the speaker profile image/name 
          on the left with his or her bio modal window**. Lorem ipsum dolor sit amet, 
          consectetur adipiscing elit. Fusce quis ornare nibh, pulvinar posuere justo. 
          Aenean laoreet nunc a eleifend lacinia. Phasellus dignissim augue at 
          consectetur ullamcorper.
        speaker: andy-escutia
      - start-time: 15:30:00 -0500
        end-time: 16:30:00 -0500
        conference: Talk Title Lorem Ipsum
        location: Conference Room C
        summary: >
          Talk's summary goes here. **You can hook up the speaker profile image/name 
          on the left with his or her bio modal window**. Lorem ipsum dolor sit amet, 
          consectetur adipiscing elit. Fusce quis ornare nibh, pulvinar posuere justo. 
          Aenean laoreet nunc a eleifend lacinia. Phasellus dignissim augue at 
          consectetur ullamcorper.
        speaker: alice-escutia
      - start-time: 16:30:00 -0500
        end-time: 17:30:00 -0500
        conference: Talk Title Lorem Ipsum
        location: Conference Room C
        summary: >
          Talk's summary goes here. **You can hook up the speaker profile image/name 
          on the left with his or her bio modal window**. Lorem ipsum dolor sit amet, 
          consectetur adipiscing elit. Fusce quis ornare nibh, pulvinar posuere justo. 
          Aenean laoreet nunc a eleifend lacinia. Phasellus dignissim augue at 
          consectetur ullamcorper.
        speaker: thomas-escutia
      - start-time: 18:00:00 -0500
        end-time: 24:00:00 -0500
        conference: Dinner & After-party
        location: Bar "La Fiesta"
        summary: >
          Lorem ipsum dolor sit amet, consectetur adipiscing elit. Fusce quis ornare 
          nibh, pulvinar posuere justo. Aenean laoreet nunc a eleifend lacinia. 
          Phasellus dignissim augue at consectetur ullamcorper.
    - date: 2024-10-18 9:00:00 -0500
      heading: Day 2
    - date: 2024-10-19 9:00:00 -0500
      heading: Day 3 and Party

  cta-group:
    - button-class: btn-primary
    link: https://rebelion.la
    text: Download Schedule
    - button-class: btn-secondary
    link: https://rebelion.la
    text: Buy Tickets
tickets: 
  intro: >
    You can use 3rd party platforms such as <a class="theme-link" href="https://www.eventbrite.com/" target="_blank">eventbrite</a> 
    and <a class="theme-link" href="https://www.tickettailor.com/" target="_blank">tickettailor</a> to sell your tickets.
  pricing:
    - name: Super Early Bird
      description: >
        Purchase before 1st Oct 2019. Only 50 tickets available. Lorem ipsum dolor sit amet, consectetur adipiscing elit.
      price: 250
      cta:
        enabled: false
        link: "#"
        text: Buy Now
    - name: Early Bird
      description: >
        Purchase before 1st June 2022. Only 100 tickets available. Lorem ipsum dolor sit amet, consectetur adipiscing elit.
      price: 350
      cta:  # enabled is true by default... testing this
        link: "#"
        text: Buy Now
    - name: Regular
      description: >
        Additional freebies and benefits included. Lorem ipsum dolor sit amet, consectetur adipiscing elit.
      price: 500
      cta:
        enabled: true
        link: "#"
        text: Buy Now
offers:
  - description: 60+ talks from industry-leading speakers
    icon: user-tie
  - description: Access to 40+ workshops
    icon: people-carry
  - description: Amazing after-parties
    icon: glass-cheers
  - description: FREE drinks, refreshments, lunch and dinner
    icon: utensils
  - description: FREE <a href="https://rebelion.la/" target="_blank">premium tees from Rebelion Labs</a>
    icon: tshirt
  - description: FREE Udemy courses
    icon: book
  - description: FREE <a href="https://themes.3rdwavemedia.com/freebies/" target="_blank">Bootstrap templates and digital resources</a> for developers worth over $100
    icon: gift
venue:
  how-to-get-there:
    description: >
      Your venue info goes here. Sed feugiat nibh lorem, a laoreet sem aliquet ut. 
      Praesent tincidunt efficitur nisi, ut eleifend diam tempor sit amet. Aliquam 
      volutpat ex feugiat, semper urna a, pharetra lacus. Sed eget eros cursus, 
      consequat lectus ultricies, efficitur metus. Sed sit amet mauris faucibus magna 
      finibus convallis vel quis justo. Curabitur ultricies sagittis erat, quis 
      faucibus lectus tempor vitae. Proin sodales, elit vitae accumsan efficitur, 
      orci quam molestie orci, accumsan tincidunt dui turpis sed libero. Duis id 
      vehicula ex. In quis pellentesque lorem, ut sollicitudin mauris.
    how-to-by:
      - title: By Plane
        description: Aliquam gravida, enim et efficitur feugiat, tellus ligula scelerisque orci, et sagittis erat lectus sit amet orci.
        icon: plane-departure
        cta:
          link: https://themes.3rdwavemedia.com/bootstrap-templates/startup/devconf-free-bootstrap-4-conference-template-for-tech-conferences-and-events/
          text: Search Tickets
      - title: By Car
        description: Aliquam gravida, enim et efficitur feugiat, tellus ligula scelerisque orci, et sagittis erat lectus sit amet orci.
        icon: car
        cta:
          link: https://themes.3rdwavemedia.com/bootstrap-templates/startup/devconf-free-bootstrap-4-conference-template-for-tech-conferences-and-events/
          text: Check Route
      - title: By Bus
        description: Aliquam gravida, enim et efficitur feugiat, tellus ligula scelerisque orci, et sagittis erat lectus sit amet orci.
        icon: bus-alt
        cta:
          link: https://themes.3rdwavemedia.com/bootstrap-templates/startup/devconf-free-bootstrap-4-conference-template-for-tech-conferences-and-events/
          text: Book Tickets
      - title: By Train
        description: Aliquam gravida, enim et efficitur feugiat, tellus ligula scelerisque orci, et sagittis erat lectus sit amet orci.
        icon: subway
        cta:
          link: https://themes.3rdwavemedia.com/bootstrap-templates/startup/devconf-free-bootstrap-4-conference-template-for-tech-conferences-and-events/
          text: Book Tickets
  facilities:
    description: >
      Your venue info goes here. Lorem ipsum dolor sit amet, consectetur adipiscing 
      elit. Proin consequat magna eu accumsan mattis. Duis non augue porttitor, 
      fringilla velit vitae, ultricies eros. Sed libero eros, tristique ac orci 
      nec, hendrerit dictum lacus. Aenean iaculis massa felis, eget venenatis 
      turpis lacinia sit amet.
    cta:
      link: https://themes.3rdwavemedia.com/bootstrap-templates/startup/devconf-free-bootstrap-4-conference-template-for-tech-conferences-and-events/
      text: Search Hotels
  # Only four are considered, if nore than 4, then others are ommited
  pictures:
    - text: Street view
      picture: assets/images/venue/venue-1.jpg
    - text: Reception
      picture: assets/images/venue/venue-2.jpg
    - text: Hall
      picture: assets/images/venue/venue-3.jpg
    - text: Pool
      picture: assets/images/venue/venue-4.jpg
sponsors:
  description: >
    Want to become a sponsor? Get in touch lorem ipsum dolor sit amet, consectetur 
    adipiscing elit. Proin consequat magna eu accumsan mattis.
  sponsor:
    - name: Adobe
      icon: assets/images/logos/logo-1.svg
      link: "#"
    - name: AWS
      icon: assets/images/logos/logo-2.svg
      link: "#"
    - name: Bitbucket
      icon: assets/images/logos/logo-3.svg
      link: "#"
    - name: slack
      icon: assets/images/logos/logo-4.svg
      link: "#"
    - name: Oracle
      icon: assets/images/logos/logo-5.svg
      link: "#"
    - name: Ionic
      icon: assets/images/logos/logo-6.svg
      link: "#"
    - name: Trello
      icon: assets/images/logos/logo-7.svg
      link: "#"
    - name: Jira
      icon: assets/images/logos/logo-8.svg
      link: "#"
    - name: Evernote
      icon: assets/images/logos/logo-9.svg
      link: "#"
    - name: Samsung
      icon: assets/images/logos/logo-10.svg
      link: "#"
    - name: Microsoft
      icon: assets/images/logos/logo-11.svg
      link: "#"
    - name: salesforce
      icon: assets/images/logos/logo-12.svg
      link: "#"
  cta:
    link: https://rebelion.la/sponsors
    text: Become A Sponsor
@endyaml
```

**References:**

* A collection of [JSON schema files](https://github.com/schemastore/schemastore/) including full API.
* [Available JSON Schemas](https://www.schemastore.org/json/)