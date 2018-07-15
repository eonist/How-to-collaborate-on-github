![](https://img.shields.io/badge/Downloads:-0-green.svg)  ![](https://img.shields.io/badge/Lisence:-MIT-orange.svg) [![codebeat badge](https://img.shields.io/badge/PDF-Coming-blue.svg)](https://github.com/eonist/how-to-collaborate-on-github/releases/package.zip) ![](https://img.shields.io/badge/Version-1.0-yellow.svg) 


### Introduction:

>A much overlooked part of software making is how we choose to organize. How we can share the amount of work evenly and keep team-mates and contributors motivated. These are some of my observations on how we can organize better on GitHub.
>

### Table of content:

1. Collaboration
    - [Asynchronous QA](#asynchronous-qa) 🤷
    - [Asynchronous issues](#asynchronous-issues) 🤔
    - [Core developer syndrome](#core-developer-syndrome) 😷
2. Automation
   - [Continuous quality](#continuous-quality) 👌
   - [Digital superpowers](#digital-super-powers) 💪
   - [Subscription life](#Subscription-life) 💸
3. Management
   - [Github for everyone](#github-for-everyone) 🌍
   - [Project hub](#project-hub) 🚦
   - [Personal career](#personal-career) 👔
   - [Feature creep](feature-creep) 😱
   - [Leaving a paper trail](#leaving-a-paper-trail)  🔍
   - [Premise of the developer](#premise-of-the-developer)  📝
   - [Simplifying complexity](#simplifying-complexity) 🗜
4. Motivation
   - [Satisfaction](#satisfaction) 😊  
   - [Incentivizing tasks](#incentivizing-tasks) 🍭 
   - [Product ownership](#product-ownership) 🔑
   - [Code debt backlogs](#code-debt-backlogs) 😅
   - [Running a tight ship](#running-a-tight-ship) 🚢
   - [Opensource as motivation](#opensource-as-motivation) ❤️
5. Shipping
 - [Asymmetrical outcomes](#asymmetrical-outcomes) 🦄 
 - [The most important feature is trust](#The-most-important-feature-is-trust) 🤞
 - [Shipping to stay relevant](#shipping-to-stay-relevant) 🚀 
 
 
 ### **TLDR;**
 >  We are all busy right? And we don’t have time for long reads anymore. That’s ok, you can just fork this book, download the pdf or star it and revisit it later. The book is about how we can stay motivated when we collaborate on github, how we can avoid feature-creep and complexity and how we can handle unrealistic expectations and deadlines. Please feel free to give feedback or suggest further reading, I can’t guarantee that it will make it in to the book, as I want it to be as succinct as possible. But it wouldn't be a very good book about collaboration if it only ever had one contributor. 🙏
 >

### **Acknowledgment:** 
> This book is still in a _very early_ stage. It revolves around the programing language `swift` but should be applicable to any programming language. It's written from the point of view of the developer as oppose to being written top-down by management. Opinions are my own and may not necessarily reflect the views of companies I work for. Please feel free to open an issue or make a pull-request if you find typos or incorrect information. License: [MIT](https://en.wikipedia.org/wiki/MIT_License) (Free & open source) 
>

# **Collaboration**

### Asynchronous issues 🤔
Prefer asynchronous collaboration over synchronous. As work becomes ever more complex and deep. Humans need less shallow focus and that means less interruption. Github handles this quite elegant through issues. Where one has to take extra care and be succinct in both asking and answering. Github recently also added edit history so one can investigate original issue and solution proposals which encourage even more diligence and less wasted mental bandwidth.

### Asynchronous QA 🤷
Questions and answers should be encapsulated in [stack-overflow-team-edition](https://stackoverflow.com/teams) 10$/mo . So that the QA isn’t lost in fleeting slack threads that may disappear forever (The free Slack account periodically wipes history). This way QA can be revisited as time progress. Instead of asking team-mates directly you can alias them `@` in SO team and also optionally ping them on slack if it's urgent (With a link to the SO team question). That way you avoid a lot of friction when having to interrupt co-workers while they are really busy solving XYZ. And your team mates gets visible credit for helping out. Just a small token like an upvote. For instance a lot of questions have to be repeatedly asked, maybe someone on your team is in charge of the backend and you have to ask him how something works and suggest upgrades. Maybe something is complicated and may break when language versions migrate to new versions and the QA needs frequent updates. Maybe many of your team-mates needs to ask the same question to the same person. At this point slack just doesn't cut it. Instead the person in charge of the backend can point in the direction of the previously answered question. Even if its related, developers can usually grasp the gist and get on with their day. Developers are very self sufficient, and often feel frustrated if they have to resort to synchronous communication. 

### Core developer syndrome 😷
If we are being honest with our selfs for a minute, collaboration is hard. Look at almost all of the top repositories on github from apple/swift, Lona, lottie, alamofire and even Atom. They all have a 1 or 2 core developers coding about 90% of the code. On the surface this is true even for something as complex as apple/swift, even though there are 4-5 people with the bulk of the commits, if you divide it up in time periods there is 1 or 2 guys doing the majority of the code. [Chris Lattner](https://github.com/lattner) solely in the beginning. Even huge open-source project such as [github/atom](https://github.com/atom/atom/)  which has 100s of contributors. It's usually a couple of core developers doing the bulk of the work. 

Company  | Project | CoreDev | Dominance | Contributors
----- | --- | --- | ---| ---
[Airbnb](https://github.com/airbnb/)  | [Lona](https://github.com/airbnb/Lona/) |  [dabbott](https://github.com/dabbott)  | 94.2% | 17
[Facebook](https://github.com/facebook)  |[facebook-sdk-swift](https://github.com/facebook/facebook-sdk-swift/) | [nlutsenko](https://github.com/nlutsenko) | 97.7% | 20
[Airbnb](https://github.com/airbnb/)  | [Lottie](https://github.com/airbnb/lottie-ios) |  [buba447](https://github.com/buba447)  | 76% | 77
[Github](https://github.com/github) |[Atom](https://github.com/atom/atom/)  | [kevinsawicki](https://github.com/kevinsawicki), [nathansobo](https://github.com/nathansobo) , [benogle](https://github.com/benogle) | 67% |  411
[AudioKit](https://github.com/AudioKit) | [AudioKit](https://github.com/AudioKit)  | [Aure](https://github.com/aure) | 92% | 81 

**Dominance**: Represents the total percentage of commits by CoreDev(s)  
**CoreDev**: The developer(s) that does the bulk of coding in a project  
**Contributors**: The total number of developers that has contributed to a project   

Being a core developer on a big project is so much more than hammering out features. As a project matures core developers will be responsible for reviewing pull requests, managing personal and external open-source projects that are used in the day to day business. Staying up to date with convention,  porting projects and it's dependencies to support the latest language API changes, writing blog posts about methodologies in order to understand them better. Writing demo projects to test new theories. Please cut them some slack if they take a bit of extra time when coding a one off submodule or a like. Their head may be a bit dispersed and they may not be as quick as a rookie developer with nothing on their plate. Doesn't make them outdated or past their prime. Apples and oranges. 🍏🍊

# **Automation**

### Continuous quality 👌
Bellow is a list of noticeable swift projects on github, sorted by code quality. As you can see popularity and big tech names doesn't always translate to great code quality. On the contrary, passion projects by indie developers such as [SindreSorhus](https://github.com/SindreSorhus) and  [3lvis](https://github.com/3lvis/)  can often yield the highest code quality.

Author | Project | LOC | Grade | [GPA](https://hub.codebeat.co/docs/gpa-explained) | Stars | [CodeCov](https://codecov.io/)
:--- | :--- | :--- | :--- | :--- | :--- | :---
[SindreSorhus](https://github.com/SindreSorhus)  | [gifski](https://github.com/SindreSorhus/gifski-app) | 788 | `A` | 3.63 | **2331** | NA
[3lvis](https://github.com/3lvis/)  | [Networking](https://github.com/3lvis/Networking) | 1110  | `A` | 3.55 |  **1100** | NA
[Eonist](https://github.com/eonist)  | [HybridCamera](https://github.com/eonist/HybridCamera)  | 756 | `A` | 3.41 | **5** | NA
[Eonist](https://github.com/eonist) | [Element](https://github.com/eonist/Element)  | 5718 | `A` | 3.38 | **815** | NA
[Linkdin](https://github.com/linkedin/LayoutKit) | [LayoutKit](https://github.com/linkedin/LayoutKit) | 4650 | `B` |   3.22 | **2557**  | 93%
[IBM](https://github.com/IBM-Swift/)  | [Kitura](https://github.com/IBM-Swift/Kitura) | 3880 | `B` | 2.96 | **6577** | NA
[Finn](https://github.com/finn-no) | [Paw](https://github.com/finn-no/Paw) | 1332 | `B` | 2.87 | **9** | NA
[AlamoFire](https://github.com/Alamofire/) | [AlamoFire](https://github.com/Alamofire/Alamofire)  | 6733  | `B`   | 2.77  | **28426**  | NA
[Apple](https://github.com/apple/) | [apple-ios-samples](https://github.com/robovm/apple-ios-samples) | 119655  | `B`   | 2.76  | **NA**  | NA
[Ramotion](https://github.com/Ramotion)  | [animated-tab-bar](https://github.com/Ramotion/animated-tab-bar)  | 719 | `C` | 2.67 | **9125** | NA
[Wordpress](https://github.com/wordpress-mobile/) | [wordpress-ios](https://github.com/wordpress-mobile/WordPress-iOS) | 92142  | `C`   | 2.61  | **2322**  | NA
[Hyper](https://github.com/hyperoslo/) | [Spots](https://github.com/hyperoslo/spots) | 7275  | `C`   | 2.55    | **1298**  | 76%
[CosmicMind](https://github.com/CosmicMind)  | [Material](https://github.com/CosmicMind/Material)  | 8266   | `C` | 2.41 | **10044** | NA
[Airbnb](https://github.com/airbnb/) | [Lottie](https://github.com/airbnb/lottie-ios) | 5433 | `C` | 2.36 | **14226** | NA
[MengTo](https://github.com/MengTo) | [Spring](https://github.com/eonist/MengTo/Spring)  | 1612 | `C` | 2.17 | **12380** | NA
[SwiftyJSON](https://github.com/SwiftyJSON/) | [SwiftyJSON](https://github.com/SwiftyJSON/SwiftyJSON) | 1037  | `D`   | 2.01  | **17172**  | NA
[Uber](https://github.com/uber/) | [UBTokenBar](https://github.com/uber/UBTokenBar) | 513  | `D`   | 1.96  | **105**  | NA
[AudioKit](https://github.com/AudioKit/) | [AudioKit](https://github.com/AudioKit/AudioKit) | 36552  | `E`   | 1.48  | **5621**  | NA

 
 
**LOC**: Lines of code (Says something about the size of the project)  
**Grade**: Corresponds to GPA. Everything over 3.3 Gets an `A` 🥇   
**GPA**: If the code is well structured, Does it avoid code smells. Is the cyclomatic complexity low. Basically says something about the code quality of the codebase. Good code quality means less bugs and less frustration when interacting with the codebase. [codebeat GPA explained](https://hub.codebeat.co/docs/gpa-explained)    
**Stars**: Correlates to how many other developers that find the project interesting / useful and wants to show their support for your OSS effort  
**CodeCov**: Indicates how much of the codebase has Continuous testing

These metrics are important. You should probably avoid adding dependencies that has a GPA grade of C. Simply because they will degrade your project. And the dependencies will struggle with bugs and complexity as time goes on and might even become impossible to work on. Humans have a tendency to pick from big house hold names and brands or whatever is recognized as being popular, it's a quick way to measure quality, but isn't necessarily wise. With Continuous Code Quality services like codebeat, Codacy or SonarCube we can pick better dependencies and learn to code better software. It's not too far fetched to think that at some point in the future GPA wont only apply to the project you work on but also to the dependencies your project relies on. Something like a dependency score. 

### Digital super powers 💪
You can create a digital product on string budget. But in my opinion you can save a lot of money by joining the SaaS eco system and paying for services that will save you time. Definitely bootstrap the MVP and ship the product to market. But once you start to form a company. Suddenly you become dependent on creating a culture that can produce high quality code. At which point it's vital to re-strap and pay for a few services that will give your developers super powers. It could mean paying 25$-100$ monthly for services but it would enable your developer team of 2-3 people to do the job of 5-6 developers. 

My modest personal service/bot budget consists of: Codebeat 20$ month, Github 7$ month, circle CI 39$ a month. I use these service to help maintain the code quality of projects i maintain and also so that I am up to date and have the in-depth knowledge required to operate these services for external clients. Small cost, high impact for both my self and companies I work for. If your more than one developer on a team it's crucial to invest in CI (Continues integration). No more: but it compiles on my machine. In this day and age almost 100% of our work is possible to do asynchronously. And as such, work that your teammates push should not be able to break CI. If it does than it also breaks everyones work and can cause multiple delays and bottle necks. Github currently has CI support for both pull requests and commits. 

In a professional project you should aim to have:  

CI | Vendor | Price  
--- | --- | ---
Continuous quality | [ Codebeat](https://codebeat.co)   | Free* (20$/m)
Continuous building | [Circle CI](https://circleci.com/)   | Free* (39$/m)
Continuous testing | [Codecov](https://codecov.io/)  | Free* (29$/m)
Continuous documentation | [Jazzy](https://github.com/realm/jazzy)   | Free  
Continuous release  | [Fastlane](https://fastlane.tools)  | Free    

`*Free for public OSS (Open-source-software)`

### Subscription life 💸
I know, I know. Subscription life sucks. But time is finite and if you can go faster you can do more in less time. Personally I don't like all these services automatically pulling $$ from my bank account. There might be inconsistencies, or credit card information may be leaked and misused. So to avoid scenarios draining my normal bank account I pay for a prepaid visa card and fill it up every quarter with 3-400$. That way if the card is defrauded I don't need to go through the hoops and legal process of trying to get back any serious amount of money. There is usually a one time fee to fill up prepaid cards, but a few dollars feels totally worth the extra level of protection it offers. It also feels more tangible to fill up the prepaid account with money on a regular basis and gives you the chance to evaluate if a service really worth it?. Sometimes the company you work for are don't want to spend pocket money on SaaS services because it adds to their overall organizational friction or they don't want to come of as careless with company funds. By personally being in charge for paying for the service your team needs, you can move faster and try more services without having to go through too much red tape. Then just take it up with billing after the fact, and explain how instrumental it was in the success of project XYZ, its always easier to ask for something when everyone is on a high note. Using anonymous visa cards also has the added benefit of leaving your personal name out of it. When shit hits the fan and the credit-card processor gets hacked and their entire database winds up on the dark web. At least your name isn't added to the increasing "personal-information-database" that is growing by the day on the dark-web. GDPR doesn't exactly apply to the dark-web. Either that or the card provider sells your info to some shady third-party ad tracking company. You know when your insta gets filled with SaaS commercials that someone sold your info. So to avoid all this, what you do is: Personal Visa -> Cash ->  pre-paid visa -> live a happy life 🏖🍸

# **Managment**
### Github for everyone 🌍
Maybe someone on your team that isn't a developer discovers a bug. Giving non-developers access to github repos enables them to: 

1. Check if a similar issue is already present, if not then [open a github issue](https://github.com/sindresorhus/gifski-app/issues/40). 
2. Ask the core dev(s) on the project, with `@` tagging, if it can be fixed. 
3. Then the developers on the project will investigate the issue discussing urgency / priority / complexity 
4. Finally assigning a priority to the issue and then with `@ tagging politely ask if someone has time to solve it. 

If the issues piles up and there are tens or hundreds of issues, then it's probably a good sign that the codebase is lacking code quality or there is lack of allocated time for maintenance of the codebase. Once an issue is fixed, the issue is closed and a link to the Pull-request that fixed the problem is added to the bottom of the issue. Keeping a tight ship is make it or break it when your building complex software involving many people / teams / dependencies. The point of all this is that the problem is presented front and center, the issue finder gets credit for finding the issue, bonus points for adding a description about what led to the error. Who ever investigates the issue and finds additional information about the issue gets credit for time spent. And finally who ever solved the problem gets commit credit. And with githubs new team commit. Everyone that was involved should be credited authors of the commit.

Let everyone be involved in making the product, its infinitely more rewarding helping building something if it's noticed and the effort is recorded and timestamped in the commit history of the project. In my opinion everyone on the team should have read and write access to all projects in the company github organization. If someone comes up with a feature that should be added then this can be added as a feature/enhancement request in the issue tracker. Tagging the issue `Help wanted` `Low/High priority`, `Question`. Adding feature as issues also has the added effect that people cant request the idea twice, because it would already be added and closed. 

Issues can have link pointers to PR's that solve them, PR's can have links to wiki posts that explain the further rational behind the Pull-Requst. Wikipages can have links to design assets in other repositories in the github organization etc. Or API documentation. Everything stored as markdown which is easily editable by everyone with full commit history of who added/edited what. 

### Project hub 🚦
Everything that is relevant in the project. API documentation, readme files, UX / Design assets. Because everything on github allows team-mates to comment and discuss changes and additions. Involving the coders in the design process of features and products are crucial when it comes to calculating the likelihood of its accomplishable or not. Not involving the person that is finally going to be making the product is a recipe for disaster both in terms of motivation and in terms of defining expectations and timeframe of completion. A workflow I enjoy on github is storing .gif .jpg and even .svg directly in a repo and using urls similar to  `https://github.com/eonist/img/master/image.jpg` and svgs via the free rawgit service: `https://rawgit.com/stylekit/img/master/FileWatcher.svg`

### Personal career 👔
I spend 100% of my working hours on github, call me a native githubber. I manage my career on github as oppose to linkdin. I get most of my freelance inquiries and job opportunities as a result of my visibility on github. Frankly github is what puts bread on my table. 
Just like how maintaining a relevant dribbble profile is crucial for a graphic designers and having songs on soundcloud is vital for aspiring musicians. Is your work impactful? Do you write with the highest standard of the industry? Education, work experience and network still counts, to a degree, but it's probably only a matter of time before unbiased CI quality bots are applied to student exams. Imagine students getting a grade seconds after they "commit" their exam. Ai bots analyzing meaning, grammar, "impact-fullness" and degree of plagiarism in nano seconds. [Like Aaron Lichtman is working on](https://github.com/alichtman) 

### Feature creep 😱
Management has a tendency to ask for additional features after features are completed by developers. Because surly after something is done the developer doesn't have anything to do. Unfortunately thats not how software building works. Piling on features only leads to complexity and bad code quality, complexity that has to be maintained. After x-amounts of features the developer responsible will have to use more and more of his time to maintain the complexity. 

### Leaving a paper trail 🔍
Managing the product development on github is crucial because it highlights what everyone is working on. On the surface make feature X and Y may seem trivial but to accomplish it issued must be solved, dependencies has to be tested and updated. CI tests have to be written, Issues must be discussed and Documentation must be written. It may very well be that in the end it takes 4 weeks instead of 2. But the crucial part is that there is a paper-trail of why and how it took twice the time that was estimated. Interacting with the complex nature of software projects is not the same as estimating more linear tasks such as painting a wall or installing a new kitchen. Sure you can always power though it and build something that resembles the specs, but not with out corrupting the overall product / code quality. Do this enough times and your left with an intertwined pile of unusable spaghetti code. That is impossible to improve or even roll back because dependencies moved on etc. By doing the entire production managment on github. Managment has full control over who does what. Github has a myriad of activity logs front and center. Both in terms of the project and individual developers that work on the project. 

<img width="644" alt="img" src="https://rawgit.com/stylekit/img/master/Screen Shot 2018-07-15 at 19.31.32.png">

### Premise of the developer 📝
If your going to run a software company it's wise to run it on the premise of the developers that are building it and the platform where it’s being built. Managers love google suite, but developers usually don’t. Developers also usually has less down time to spare than managers and support staff. Developers usually operate at 100% cognition where as managers often has a lot of down time between meetings and organizational work.


### Simplifying complexity 🗜
Keeping documentation where the projects are built. Instead of putting documents on google, api instructions on slack , UX pdfs on a google drive, and issues in basecam. One should rather collect it in the place where the digital product is being built. Github caters to all the needs described above. Documents can be collaboratively written in the wiki section, complete with commit history etc. You can even update wikis from the comfort of your favorit text editors as the entire wiki section is a .git repo in it self. Issues should be documented and discussed in the issue section. Design assets can be version controlled in it's own repo through [kaktus](https://kactus.io/)  instead of in emails / dropbox. The great thing about collaborating on github is that no resolution is lost, all efforts are version controlled. It's also the industry standard when it comes to building software so everyone (should) know it as if it was the back of their hand. Learning Markdown is also vital. Learning markdown takes a few minutes and is a lot of fun to master ;) 

# **Motivation**

### Satisfaction 😊
Committing code is a little like chopping wood. After a long and sweaty day among trees, struggling with bugs and tooling that fails you when you least expect it, you finally see the result as a stack of lumber, which closely translates to a stack of commits in the digital realm. One on piece of wood stacked on top of the other. It's a satisfying sight to behold. Some lumps are thorny and still have twigs sticking out. Similar to how some commits are rough around the edges and could be improved with some pruning. The end result of your hard work is visible to the naked eye, and you have something to show for your hard work, something to show management, co workers and your self. A chunk of work written into the history of the project, something tangible that says something about who you are, what choices you made, what shortcuts where taken and exactly how much elbow grease you put into it. 2 weeks of work that can be investigated, probably something you wont be proud of 2 years from now but that doesn't matter. The work is there for your entire company to see and it will fuel your motivation in next endeavor you take on. Sometimes your work is applauded other times its criticized and improvements are suggested by your colleagues and peers. Yet other times you can feel like your head is always tipping under water, and your struggling to breath because the tasks keep coming in and your having trouble finding a foothold to keep up with the ever increasing complexity and scope. Estimating tasks starts to become difficult, but by using the commit history and pull-request comment threads from the last completed task you are able to give a more accurate estimate. Maybe there were bottlenecks you had to overcome like happened in commit id: `dv7e22` and also in `ku3ce`. Estimates are complex, and are increasing in complexity as a project grows. Simply asking for estimates doesn't cut it anymore. Management has to be integrated in to the platform where the work happens, not simply be asigners and time keepers. Non-techinical managers needs to keep up with the times and learn how to look under the hood (aka read” commit descriptions) and be able to understand consequences of organizational friction and how "feature creep" has a tendency to lead to bottlenecks when developing software. The image bellow is from my recent experience with wood chopping. I estimated id complete it in a weekend, but in the end it took 10 days. Doing something the first time always takes longer than you expect, but every time I walk by it It feels satisfying to look at. 💪 

<img width="600" alt="img" src="https://rawgit.com/stylekit/img/master/Screen Shot 2018-07-10 at 16.31.53.png">


### Incentivizing tasks 🍭 
Stackoverflow is great. It incentives people to help other people on the off chance that someone in the future may upvote your the effort to help. Every time I need to look up some code related issue i fire up chrome with stackoverflow and see if I can find something related to my code question. Sometimes there is a little green flag that indicates a few of my previous answers has been upvoted since i last visited the site. And other times there is a red flag indicating that someone has additional questions, maybe I have to adjust one of my answers to reflect recent API change etc. stackoverflow isn't with out flaws, there is no incentive to change previous answers by other people that clearly needs an update, People are rather incentivesed to add new answers of their own, often duplicates of previous answers. and as a result you end up with slightly different variations of the same answer. Instead one could have just updated the original answer.but since there is no upvotes to be gained for edits and since no one will ever know you updated the answer. People simple avoid doing things that are not noticed or adds up to their personal prosperity. 

### Product ownership
Organizing your product development on github also highlights who does what, and their impact on what is being made. Parts of the product can be branched of to opensource mini projects that emplyees can be "product-owners" of. There is empircal eveidence that so called product owners are order of magnitudes more productive than emplyees that dont feel any ownership. even if that ownership is ephemeral and limited in time, the likleyhood of a better outcome is 10x higher than if product ownership is fleeting and watered down between individuals. People just dont care about products they dont get credit for. As a piece of anecdotal evidence take spotify as an example. Spotify has begun making job ads with Digital productowner in the title. because they experience employees feeling dissatisfied in their working condition and are leaving for other more satisifing ventures where they can get more credit for their efforts. Its also evident in spotifys productline. Take the webplayer for instance. Even something as basic and simple as pressing the play button doesn't work. You have to press it over and over, often refreshing the browser, and waiting a long time until it finally plays the wrong song. How hard can it be? why are they not fixing this simple issue? As It turns out the inter organization ticketing system isnt working. To fix the issue you have to coordinate who ever made the webplayer interface and then who ever made the mobile player. because the mobile player needs to be pause to make it possible for the the desktop player to start. Because its neat feature that they interact. If it worked. So now you have two units that has to coordinate to fix a problem that is pretty trivial. But the units are busy on project XYZ that are more important for their career and personal outcome. and so are not motivated to fix the issue. so it remains unsolved until the next batch of employees re-write everything. 

### Code debt backlogs 😅
One has to ask. If this was my personal codebase on a personal project what would I prioritize coding? The mundane issue that improves the stability of the app and has exponential value in simplifying further coding, but that no one visibly notice or knows about? or adding new flashy features that management understands and can visibly see. Something that feels like progress. On a personal project the former is a no brainer. On collaborative projects the latter 99% of the time gets prioritized, because visible progress. never mind the 100+ backlog issues and code debt. A worry for another time. until the codebase crawls to a stop not even updating a simple style is possible without weeks/months of effort. 


### Running a tight ship 🚢
creating an issue, and trying to solve it. sometimes some strange bug can take a while to resolve. highligthing why what and when is key to explaining why the other deliverables are late. causuality. but its allabpart of a good keeping a tight ship. and good grounds keeping. its also about leaving  a papertrail. when managment get a bit too exuberant and ask a bit too much, and you as a dev dont want to be a party stopper and go with the flow. maybe you cant finish what they ask, but maybe just starting something is gd enough, and then leave it up to managment to invest more into to it. 


### Opensource as motivation ❤️
In my opinion encouraging employees to write opensource modules has a great effect on the productline for your company and the motivation of the emplyee. The dymaics is something like this: Employees that are allowed to write opensource modules just care more about what they are building, they have a stake in the overarching outcome of the company that is beyond money. Different people have different motivators. Some are actually motivated by money, some are founders at startups and are motivated by getting their business sold and cashing out. Most likley your a regular employee at a company doing what you can to help the company excel. Humans are usually driven by small incentives and dreams. In a sense Github motivates you to get up in the morning and write a test for things you know no one is going to care about. At least you can open-source it and maybe get some exposure and interest from other developers. Maybe even land your next job. Github's infamous commit-graph streaks also motivates you to keep hustling. I totally respect devs who has blanks for saturday and sundays like [Josh Harber](https://github.com/joshaber) . To be honest whenever I see that i think the world is a better place. Ideas are fueled by dreams and aspirations. A motivated developer has a lot more impact than someone that is there just for the sake of having a job. Thats why its really important that developers are included when the concept is created. Instead of just being given tasks from top down. It should rather be the developer that assigns him self tasks.

# **Shipping**

### Asymmetrical outcomes 🦄
Build something epic and they will come. On the contrary, Sindre Sorhus as built a reputation for building software over time. slowly building traction and publicity around what he makes. Meticulously churning out small improvements to obscure modules that makes up the array of digital products he now manage in his github profile. Sindre has understood that products doesn't have to be shipped when they are ready, but are rather shipped over time, with live feed-back as [bugs present them selfs](https://github.com/sindresorhus/gifski-app/issues/40). Popularity and success are properties that usually arrive very asymmetrically. Sindre has understood that many small streams can form a big river. His currently at nr.13 on the [global-github leader-board](http://git-awards.com/users) in front of Trillion dollar conglomerates such as Apple, Microsoft and Google. Everything that he codes/writes/supports adds to the overall feedback loop of his umbrella organization, spanning 100s of developers from all over the world chipping in for free, all the while he masterfully manages it all on github usually from a cafe in Thailand. 🏝🍹

### The most important feature is trust 🤞
Building a github profile is also about trust. Would you rather use a free closed source app from a random developer on the AppStore. Or would you use an OSS app from github by sindre sorhus, which depends on maintain his reputation that he has built over many years, and if where broken could probably never rebuild again. In this day an age where it’s getting harder and harder to make money from apps many devs are tempted to syphon a little private information or even worse install backdoors or spam-ware.

### Shipping to stay relevant 🚀 
With AI on the horizon and a shrinking pool of available jobs. Maintaining a relevant github profile is more important than ever. Technology moves faster and faster and people that stops shipping relevant projects will be replaced by someone with more relevant abilities. There is a theory floating around that humanity will come up with new jobs once the superfluous jobs disappear. I guess time will tell, but in the mean time staying relevant is all we can do. 
