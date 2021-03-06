# Teraskos Documentation
```
Repo ini digunakan untuk mendokumentasikan repo yang ada, guide, atau stack yang kita akan gunakan nantinya,
berikut standarisasi dan flow untuk berkontribusi untuk setiap repo yang ada.
```
#### 10-12-2020
```
Keperluan saat ini adalah Endpoints dan Landing Page, 
jadi page ini sementara diutamakan untuk memetakan keperluan 
yang akan digunakan untuk mengembangkan API dan Landing Page.
```
## Index
1. [TeraskosDEV Team Member](#teraskosdev-team)
1. [Architectural Overview](#architectural-overview)
1. [Front End Stack](#front-end-stack) 
1. [Back End Stack](#back-end-stack) 
1. [Valuable Tools](#valuable-tools) 
1. [Contribution Guide Resource](#contribution-guide-resources) 

## TeraskosDEV Team
List developer teraskos, digunakan untuk mention/assigning nantinya jika ada issue terkait perkembangan teraskos.

- [@saveroo](https://github.com/saveroo)
  - Bertugas memanage & mendokumentasikan keperluan technical
  - Berikut arsitektural untuk menunjang project ini.
- ...
- 

## Architectural Overview
Flow overview

- Relation
  - Back-End
    -Admin
    -Landing Page
  - Admin
    -Back-end
  - Landing
    -Back-end

- [Landing-Page] Should be Independent framework/lib agnostic.
- [Landing-Page] Consuming the data from Back End
- [Landing-Page] Doesn't have relation with Admin Page

- [Admin-Page] Should be Independent and framework/lib agnostic.
- [Admin-Page] Should be able to Create/Read/Update/Delete via Endpoint

- [Back-end] Endpoint should have it's own responsibility.
- [Back-end] Should follow (SDD) Schema-driven development to change stack if neccessary.
- [Back-end] Will be core endpoint for now, following monolithic patterns
- [Back-end] Back-end will process the data from Admin page.
- [Back-end] Back-end will process the data from Landing page.
- [Back-end] Should be Database Agnostic, we use STRAPI, should be fine.

  
## Front-End Stack
Saat ini hanya untuk perluan landing page

- __[Landing Page]__
  - [JS Library]
    - Next.JS (React)
    - Redux/React Hook (Untuk state management)
  - [CSS Library] tidak untuk digunakan keduanya, namun pilihan yg akan kita decide nantinya.
    - [TailwindCSS](https://github.com/tailwindlabs/tailwindcss)
    - [ChakraUI](https://chakra-ui.com/)
  - [Packages && Resources]
    - [No Lodash](https://youmightnotneed.com/lodash/)
    - [ESLint Airbnb/prettier Standard]
  - [Deployment] (perlu saya konfirmasi dahulu sama yg sebelumnya memegang)
    - Serverless
      - vercel
      - firebase
      - heroku
  - [TODO LIST]
    - [ ] Bootstraping Next.JS Project at [teraskos-web](https://github.com/teraskos/teraskos-web)
    
- __[Mobile??, Silahkan diisi]__

## Back-End Stack.

  - [TODO LIST]
    - [] Initialize STRAPI Project at [teraskos-api](https://github.com/teraskos/teraskos-api)

## Valuable Tools
- [Insomnia Core (Postman Equivalent)](https://insomnia.rest/)
  - Used for API Testing
- [Insomnia Designer (OPEN API Specification) to help building API](https://insomnia.rest/download/#linux)
  - Used for designing Endpoints and testing based on defined schema.
- [FIGMA](https://figma.com/download/)
  - UI Design Proposal
- [Play Tailwind](https://play.tailwindcss.com/)
  - Setelah UI design coba bisa di implementasikan disini dahulu untuk prototyping komponen.

  
## Contribution Guide Resources
- [Gitmoji](https://gitmoji.carloscuesta.me/)
  - Untuk commit message, cth: "feat(:tada:): implement A logic."
- [Conventional Commit Message](https://www.conventionalcommits.org/en/v1.0.0/)
  - Tolong dipelajari untuk, tidak harus, tapi akan lebih baik jika dapat meng implementasikan.

## General TODO

- []
- []
