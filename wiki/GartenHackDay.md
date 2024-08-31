:::lead
It is in our DNA to [[SelfIntroduction|create]] build things. A Garten Hack Day is an [[informal gathering]] for us to build [[public by default|public]] tools for internal use.
:::

# Upcoming

# 2024-08-31

- **Inventory tracking** ({% render 'Person', name: 'dtinth' %}, {% render 'Person', name: 'rayriffy' %}): Building the tool and produce labels so we can identify which equipments belong to Creatorsgarten and which are not.

    - {% render 'Person', name: 'rayriffy' %} updated {% render 'GitHub', repo: 'creatorsgarten/inventory' %} to use Biome, implemented the UI for adding items. {% render 'Person', name: 'dtinth' %} migrated the DB migration system from Supabase to use Drizzle Kit (the app still runs on Supabase). We printed more stickers and flags to attach to our [equipments](https://inventory.creatorsgarten.org).

- **Event photos**: {% render 'Person', name: 'faypichaya' %} raised an issue about event photos management “รูปอีเว้นในงานนี่ทีมเรามีวิธีเก้บอะไรมั้ย หรือโยนเข้าไดฟ์ปกติเลย”. Maybe we should consolidate the public event photos so people can find the photos of past events.

- **Image management** ({% render 'Person', name: 'dtinth' %}): ~~I am thinking about image hosting solutions, right now images are hosted on GitHub / Discord / Thai’s R3 bucket.~~ I built a system to upload images to Cloudinary after got inspired from talking with Cloudinary people at CityJS Singapore. However, this system is not integrated with our wiki editor yet.

- **Wiki editor** ({% render 'Person', name: 'rayriffy' %}): Riffy has an idea for improving the editor using [Plate JS](https://platejs.org/).

- **Insta360 Link websockets protocol reverse engineering** ({% render 'Person', name: 'dtinth' %}, {% render 'Person', name: 'rayriffy' %}): Insta360 Link Controller software version 1.4.1 supports remotely controlling the webcam using a web interface on the phone. From preliminary inspection, it is using the WebSocket protocol but the messages are binary format. The goal is to decipher this format and allow us to programmatically control the camera. Combined with Chrome’s [FaceDetection](https://developer.chrome.com/docs/capabilities/shape-detection#facedetector) API, we may be able to improve the face auto-tracking algorithm so that we (as the livestreaming crew) don’t have to babysit the camera as often.

- For {% render 'Event', name: 'javascriptbangkok2' %} and other future Creatorsgarten events:

  - **Live transcription system** ({% render 'Person', name: 'dtinth' %}): Experiment with how we can live-transcribe a tech talk. English language is pretty much solved (thanks to Speechmatics) but Thai language talks has a lot to experiment and research.

  - **Check-in experience** ({% render 'Person', name: 'dtinth' %}): Play with a hardware barcode scanner.