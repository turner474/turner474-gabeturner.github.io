## November 13, 2025 pt2

* The Pi os corrupted somehow! Yay, have to reflash... not a big deal there's nothing important on the pi but still annoying... 

## November 13, 2025

* Still trying to get the model to work decent on the pi
* Hope to finish that by today and can implement this laughably bad 'flame sensor' that maxes out at 2 feet.
* At least can test out the wake interrupt logic
* Think that part of model running so terribly slow is that it was headed w/ a window... which is neccassary for testing but not so much for use, so think ill dial headed on laptop then headless on pi with just text output after figuring out the fastest format



## November 12, 2025

* Still working on optimizing the model for RPi
* Works great on my laptop through webcam, not so much on the pi... talking sub 2fps...
* Playing around with different model formats and lite versions video compression etc...

## November 11, 2025

* Had to take some time for more pressing things... exams and internships
* Ebay seller cancelled order after 11 days of nothing... so that sets me behind a bit.
* Ordered new UV bulbs from seller in America so hopefully will arrive soon, driver board is on my desk just need bulbs
* Ordered special board for CV-hope to migrate off the Pi to that, given its smaller more power efficient and will hopefully allow for battery prototype. Should be better for higher CV fps, however today im working on optimizing the model for the Pi still.
* Converting from yolo8 to onnx... then will play around with image size/quality in a virtual ubuntu enviorment because doing that through ssh on the pi is annoying.
* The goal is that the bulbs will come soon, I can dial in the model and wake interrupt on the pi, and then migrate into the new board (Maix II) and have a 3D printed housing plus battery for BDM comp. demo in December.

## October 28, 2025

* Studying perceptron and classification for exam tomorrow, got bored, decided to implement ML classification today!
* Wanted to run it all on RPi, but Mediapipe isn't supported in env.
* Anyways... Took two videos of myself, one with flame one without, from a camera on the RPi, through HTTP.
* Spliced both videos into 2frames images, spent a while labeling said images for fire
* Trained a YOLOv8 model on annotated images for 50 epochs
* Really pleased with model-given training data is so minimal... like 50 flame image highlights
* Combined with mediapipe on my computer for human feature recognition
* ...Boom, we have actual safe/unsafe flame classification... yay!
* Took a video threw it on the website. Now I will study for my exam again!

## October 26, 2025

* Got the website looking a bit better...
* Made showcase/demo videos for site.
* Ordered UV sensor + driver board.
* Worked on configurations for future prototypes-migrating from RPi.
* Need to study for exams while waiting for parts!!!

## October 25, 2025

* Filed provisional patent application.
* Published GitHub website for Ember/Cedaris.
* Updated notes structure and layout for tracking ongoing work.
* Need to work on brand image and trademark
* Worked on trying to get the camera I bought to work... after extensive testing I've concluded MISO is stuck high. In my earlier attempts I must've carelessly connected to 5v or something. Another camera (more compatible) can be found on amazon and will be bought today.
* The solar blind UV bulb I want is expensive and needs supplemental hardware. I worked with a simple 8x8 thermal array and a temperature threshold to determine flame latency/detection time.
* The 8x8 is almost completely irrelevant for actual use cases at distance, but might as well continue working though concepts while parts come. The 8x8 only works to about 5 inches in low light and 6 at high light, but generally averaged about a half second, from flame to alert, which if I can replicate with UV at distance I would be pretty pleased.
* https://docs.google.com/spreadsheets/d/1mN5ks6RynumLbIRvH-owR4nm6jO64EUpij71O\_HHEjY/edit?usp=sharing <- data

## October 24, 2025

* Meeting with AI Professional @ Schwab:

  * Advised reading *Million Dollar Weekend* and starting quickly.
  * Emphasized quantifying demand and preorders.
  * “AI demand > people who know AI.”
  * Encouraged launching publicly before perfecting product.

* Scheduled Purdue Incubator meeting.
* Finalized provisional patent and drawings.
* Prepared for filing and payment.
* Realized drawing process improved product definition.
* Created GitHub website and continued developing provisional package.

## October 23, 2025

* Applied to Purdue Incubator (awaiting feedback).
* Realized Ember would fail to send alerts during electrical fires if Wi-Fi is down.
* Dropped thermal sensor from MVP due to redundancy and battery limits.
* Brainstormed no-Wi-Fi hub concept:

  * “Ember Hub” device to relay alerts to datacenter and EMS.
  * Decided it’s probably unnecessary for MVP but could be a future add-on.

* Model after Ring’s business strategy:

  * Define problem Ember solves.
  * Prioritize ease of installation and minimal friction.
  * Plan to expand sensors after core product is proven.
  * Focus on brand image, RR is good, but I do not want to monetize alerts.

* Began work on marketing copy, website setup via GitHub, and continued provisional filing prep.

## October 21, 2025

* Hardware prototyping:

  * Decided prototype should start with Raspberry Pi, later migrate to custom industrial-grade board.
  * Considered part tradeoffs (e.g., R13192 vs. R9533 for cost).
  * Planned to finalize design specs, including PCB fab possibilities.

* Market research planning (“ask people: how much would you pay?”).
* VC vs. non-VC funding considerations.
* Realized current hardware costs for prototype may reach ~$500+ (UVTRON, IMX678, etc.).
* Decided wireless approach preferred over wired integration.
* Planned to explore battery feasibility through interrupt wake logic.
* Books to read: *Prototype to Product*, *The Hardware Startup*.
* Contacted Purdue Innovates for potential support.

## October 20, 2025

* Patent strategy thoughts:

  * Focus patents on technology that supports customer experience.
  * Prioritize provisional filings that stack logically.
  * Build around the “why customers love the product.”

## October 19, 2025

* Worked on provisional patent (UV + Thermal + CV sensor system).
* Considered Purdue IP resources and clinics.
* Patent naming brainstorm: *EMBR*, *Ember*, *Aember*, *EmberSense*.
* Noted: Provisional only protects what is explicitly included; claims in conversion app must be supported.
* Considering trademark intent-to-use filing; specimen can be submitted later.
* Deferred full patent filing until clearer prototype and specs.
* Concept development: Tri-model fusion (CV + IR + Thermal).
* Strategy:

  * Wait to file as long as possible.
  * File before public disclosure.
  * Focus current effort on prototyping instead of filing.

* Evaluated production costs and hardware feasibility.

  * Current idea: UVTRON + CV + IR sensors.
  * Privacy considerations (“no big brother” vibe).
  * Desired on-device CV processing.
  * Began thinking about battery capacity, range, and component layout.

* Questioned need for electrical engineer; decided to progress prototype independently for now given capital limitations.
* Bought MQ gas sensor; planned to begin bookkeeping.

## October 18, 2025

* Could not get Arducam to work (bought Pico version by mistake).
* Got smoke detector with beeper working.
* Planned: Market research and design refinement for trademark.
* Decided to focus more on thermal sensor work.
* Considered UV sensing but deemed it not viable versus IR.

## October 17, 2025

* Began prototyping phase.
* Tested thermal sensor (working, but requires extensive testing).

## October 16, 2025

* Planned updates: Secretary of State, IRS, and business license.
* Generated Operating Agreement.
* Began outreach

## October 15, 2025

* Named Cedaris Technologies LLC (derived from "Cedar" + Latin suffix).
* Filed initial LLC paperwork.
* Initial list of managers.
* Drafted Operating Agreement.
* Planned to open business account (Mercury, Relay, Novo, or local).
