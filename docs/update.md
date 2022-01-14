---
editLink: false
---
# An update from the Faker team

_January 13th, 2022_

:wave: We're pretty excited to give new life to this project.

We want the project to have a fresh start and become _even cooler_.

::: tip Note
Given the attention this library has gotten outside of the JavaScript community, I'm assuming nothing about the audience of this statement.
:::

[[toc]]

## What is Faker?

Faker is a library that generates fake (but reasonable) data for you. Mock data. Data for testing, development, and the like.

**Faker was first implemented in Perl in 2004 by Jason Kohles** ([he reached out to us in support 💛](https://github.com/faker-js/faker/discussions/55)), and has since been ported to _many_ languages including [Ruby](https://github.com/faker-ruby/faker), [Python](https://faker.readthedocs.io/en/master/), [Java](https://github.com/DiUS/java-faker), [Clojure](https://github.com/paraseba/faker), and [PHP](https://fakerphp.github.io/). 

This is the JavaScript port.

## I heard something happened. What's the TLDR?

The Faker project was maintained by Marak Squires, an early-days impactful Node enthusiast and professional who went rogue and acted maliciously on January 4th, 2022.

We're now turning Faker into a _community-controlled project_ currently maintained by _eight_ engineers from various backgrounds and companies.

::: tip From the news
For more information, here are some major news articles that covered what happened:

[The Verge](https://www.theverge.com/2022/1/9/22874949/developer-corrupts-open-source-libraries-projects-affected), [Bleeping Computed](https://www.bleepingcomputer.com/news/security/dev-corrupts-npm-libs-colors-and-faker-breaking-thousands-of-apps/), 
[The Register](https://www.theregister.com/2022/01/10/npm_fakerjs_colorsjs/), [ZDNet](https://www.zdnet.com/article/when-open-source-developers-go-bad/), [Naked Security](https://nakedsecurity.sophos.com/2022/01/11/javascript-developer-destroys-own-projects-in-supply-chain-lesson/).
:::

## Is it called Faker or faker.js?

We try to call it Faker in the code and in titles, but faker-js is more available as a username.

## Is this the official library?

I'm referring to it as the official library in the immediate term in order to disambiguate between the many rewrites and forks that are not community-maintained. We'll drop "official" once things have died down and there's less chaos around the library in general.

## _________ is also working on a Faker library

Please send them to our [Discord](https://discord.gg/k4bPM5dzqC) and we can share ideas and collaborate.

## Who are the current maintainers?

We're a group of engineers who were using Faker in prod when the main package was deleted.

We have eight maintainers currently.
* Damien Retzinger - [GitHub](https://github.com/damienwebdev), [Twitter](https://twitter.com/damienwebdev)
* Shinigami - [Github](https://github.com/Shinigami92), [Twitter](https://twitter.com/Shini_92)
* Daniel Bannert - [Github](https://github.com/_prisis_), [Twitter](https://twitter.com/_prisis_)
* Erica Clark - [GitHub](https://github.com/clarkerican), [Twitter](https://twitter.com/clarkerican)
* Mo Mahallawy - [GitHub](https://github.com/mmahalwy), [Twitter](https://twitter.com/mmahalwy)
* griest - [GitLab](https://gitlab.com/griest)
* Mateus Dadalto - [GitHub](https://github.com/MateusDadalto), [Twitter](https://twitter.com/MateusD)
* Jessica Sachs - [GitHub](https://github.com/JessicaSachs), [Twitter](https://twitter.com/_JessicaSachs)

## What has the team done so far?

1. Created a [GitHub org](https://github.com/faker-js/faker) for the new faker package under `@faker-js/faker`.
2. Put together a team of **eight** maintainers.
3. Released all previous versions of faker at `@faker-js/faker` on [npm](https://npmjs.com/@faker-js/faker).
6. Started development on version 6.
7. Almost completed migrating to TypeScript so that DefinitelyTyped no longer needs to maintain its external [@types/faker](https://www.npmjs.com/package/@types/faker) package.
8. Created a public [Twitter](https://twitter.com/faker_js) account for communicating with the community.
9. Released the first official Faker [documentation](https://fakerjs.dev) website.

::: tip Thank you Jeff!
Faker has never had an official docs website and the awesome [Jeff Beltran](https://github.com/JeffBeltran) has been maintaining a project called "[Un-Official faker.js Documentation](https://github.com/JeffBeltran/faker.js-docs)" for the last 3 years. 

He gave us permission to re-use his work to create **[fakerjs.dev](https://fakerjs.dev)**
:::

8. Cleaned up tooling like Prettier, CI, Netlify Deploy Previews, and GitHub Actions.

9. Done a TON of issue triage and many, many PR reviews.

<div style="text-align: center;"><img src="./public/first-week-wins.png" width="600" alt="64 pull requests were opened. 34 were merged. 44 issues were opened. 25 were closed." /></div>

10. We've gotten in contact with the [Open Collective](https://opencollective.com) and discussed a transition plan for the project.

## Is there a roadmap?

I wrote this up somewhere else, but this is not a copy + paste project.

**This is a fork for backwards-compatibility only**.

We fully intend to extend Faker, continuously develop it, and make it _even better_. 

As such, we will work on a roadmap after we release 6.x and merge all of the TypeScript Pull Requests in the next week.

Some of the items on our roadmap:
1. ESM Support!
2. Browserify => Rollup/Vite
3. Improved testing infrastructure
4. typegen docs
5. Engage with existing maintainers of the Faker ecosystem
6. Interactive Playground within the docs
7. Node 18 compatibility

## FUNDING.yml

When we opened the repository, we received an influx of issues to remove Marak from the `FUNDING.yml`. [#15](https://github.com/faker-js/faker/pull/15), [#43](https://github.com/faker-js/faker/pull/43), [#110](https://github.com/faker-js/faker/pull/110), [#111](https://github.com/faker-js/faker/pull/111), [#112](https://github.com/faker-js/faker/pull/112)

We were closing issues every other hour. Discussing the `FUNDING.yml` was inevitable. We pushed it off for four days so that we could focus on re-establishing the health of the project in service of the community.

When we became aware that this project was the most stable fork of Faker with the most community support, we realized that we needed to deal with the `FUNDING.yml` file and take a stance.

:::tip Short version, please
I posted a [concise and thorough writeup](https://github.com/faker-js/faker/discussions/56#discussioncomment-1958057) of the logic behind our actions and decisions.

This was backed by the support of all of the co-maintainers. It's a much less narrative version of this section, so if you want the TLDR and some photos of the transactions, give it a read.
:::

We discussed and we came to the determination that users unfamiliar with the whole faker situation wouldn't know that the repository's sponsorship links aren't funding the continued development of the project.

Faker is funded by an [Open Collective](https://opencollective.com/fakerjs), and so on January 12th, 2022, I contacted Ben Nickolls, the Executive Director at Open Collective.

During the conversation with Ben, he went over the terms and conditions of the Open Collective with me.

He said that simply, "The funding is attached to the project, not the maintainer."

I went back to the team and each maintainer stated what they wanted to happen. Unanimously, we agreed that we **wanted absolutely no ability to touch the existing funding**.

We created a cut-over plan with the support of Open Collective.

:::tip Old collective
There is now a [fakerjs-legacy](https://opencollective.com/fakerjs-legacy) collective. Open Collective transferred all funding into the legacy account and invited Marak + the other maintainer, Brian, into the _legacy_ collective so that they could do whatever they wanted with the funds.
:::

After the funds were moved we were invited to become admins of the Faker collective. This meant that *we retained the existing sponsors* of the [Faker](https://opencollective.com/fakerjs) collective who were paying for the continued maintenance of the project.

We believed that this was the most equitable and transparent way to act both for supporting our sponsors who want to pay for the project _and_ for ensuring that Marak and Brian are able to cash out for the hard work that they've put into the project.

Due to Open Collective's transparent systems, you can visit the fakerjs-legacy collective's [transactions](https://opencollective.com/fakerjs-legacy/transactions) to see the deposit of `$11,652.69 USD`.

::: tip SPONSORING MARAK
For those who were sponsoring the fakerjs open collective as a way to personally sponsor Marak, please donate to the [fakerjs-legacy open collective](https://opencollective.com/fakerjs-legacy).

An e-mail from our team will also arrive in the next few days notifying Open Collective sponsors that the maintainer team has changed.

We have no information with regards to his GitHub Sponsors.
:::

## How will the team operate financially?

I reached out to Ben Nickolls, the Executive Director of Open Collective to get advice.

He had two recommendations:
1. To do what ESLint is doing. "[A year of paying contributors: Review](https://eslint.org/blog/2020/10/year-paying-contributors-review)" 
2. To join the free workshop that Open Collective has recently started. "[Deciding on how to use your money](https://opencollective.com/workshops/events/deciding-on-how-to-use-your-money-020765bf)".

**Those are the models we will follow**.

## In closing...

We're excited to give new life to this idea and project.

This project **can** have a fresh start and it will become **even cooler**.

We felt we needed to do a public announcement because of all of the attention the project received in the media and from the community.

We believe that we have acted in the way that is best for the community.

We will continue to work on the project and not only maintain it, but actively develop new and awesome features.

_\- Jessica Sachs and the Faker Team_