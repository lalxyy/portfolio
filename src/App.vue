<template>
  <div id="app">
    <Layout>
      <Header style="background: white;">
        <Row>
          <Col :span="12">
            <div style="display: inline-block;">
              <h3 style="margin-left: 10px;">Ang (Carl) Li</h3>
            </div>
            <div style="display: inline-block; margin-left: 20px;">
              <Menu mode="horizontal"
                    style="display: inline; margin-left: 10px;" theme="light">
                <MenuItem name="myself" to="#me">
                  Me
                </MenuItem>
                <!--<MenuItem name="projects0" to="#projects">-->
                  <!--Projects-->
                <!--</MenuItem>-->
                <Submenu name="projectmenu">
                  <template slot="title">
                    Projects
                  </template>
                  <MenuItem name="ideaman" to="#ideaman">
                    IdeaMan
                  </MenuItem>
                  <MenuItem name="shenma" to="#shenma">
                    Text Classification in Alibaba Group
                  </MenuItem>
                  <MenuItem name="peterbook" to="#peterbook">
                    Peterbook in UCSD
                  </MenuItem>
                  <MenuItem name="mediavault" to="#mediavault">
                    Media Vault Website
                  </MenuItem>
                  <MenuItem name="vspace" to="#vspace">
                    VSpace (Campus App)
                  </MenuItem>
                </Submenu>
                <!--<MenuItem name="side">-->
                  <!--Side Projects-->
                <!--</MenuItem>-->
              </Menu>
            </div>
          </Col>
          <Col :span="12">
            <div style="position: absolute; right: 0;">
              <div style="display: inline-block;">
                <Menu mode="horizontal"
                      style="display: inline; margin-left: 10px;" theme="light">
                  <MenuItem name="github" to="https://github.com/lalxyy" target="_blank">
                    <Icon type="logo-github"/>
                    GitHub
                  </MenuItem>
                  <MenuItem name="linkedin" to="https://www.linkedin.com/in/lalxyy" target="_blank">
                    <Icon type="logo-linkedin"/>
                    LinkedIn
                  </MenuItem>
                </Menu>
              </div>
            </div>
          </Col>
        </Row>
      </Header>
      <Content>
        <div style="margin: 20px 100px;" id="me">
          <div>
            <Row :gutter="50">
              <Col :span="3">
                <img :src="images.myPhoto" alt="My Photo" style="border-radius: 50%; width: 100%; margin-top: 0;" />
              </Col>
              <Col :span="21">
                <p>I am now a senior undergraduate in Northeastern University, China, meanwhile a research assistant and tech lead in recommender system lab in my undergraduate college. I am a Full Stack Developer with proficiency in Python and JavaScript, meanwhile have experience in PHP, MATLAB, R and Java EE. In the past time I was an algorithm engineer (NLP) intern in Alibaba Group, Hangzhou, China; previously an exchange undergraduate at University of California, San Diego (UCSD) and undergraduate of Northeastern University, China. GPA 3.9/4 in UCSD, 87/100 in NEU (China).</p>
                <p style="margin-top: 20px;">During my previous internship in Alibaba, I'm excited that my text classification model could be used by millions of users of UCWeb, making UCWeb understand more of its users and contribute much more valuable content to them. Through this experience I realized that my knowledge and techniques could make the world a little better through my efforts. I'm really pleased with that. Now, working as a research assistant in Northeastern University, China, meanwhile member of the lab's most successful project LibRec, I am leading a small team to build a web community called IdeaMan, in order to help researchers around the world build research networks or even find potential research opportunities. I believe that's another way for me to realize the dream of making the world better through technology.</p>
              </Col>
            </Row>
          </div>
          <div style="margin-top: 30px;">
            <h2 id="projects">Projects</h2>
          </div>
          <Card style="margin-top: 20px; font-size: 12pt;" id="ideaman">
            <div slot="title">
              <Row>
                <Col :span="12">
                  <p>IdeaMan</p>
                </Col>
                <Col :span="12">
                  <p style="text-align: right;">Northeastern University, China</p>
                </Col>
              </Row>
            </div>
            <div>IdeaMan is a web community utilized by our lab's project <a href="https://github.com/guoguibing/librec">LibRec</a>, a leading recommender systems library with 2,000 stars on GitHub, in order to help researchers around the world build research networks or even find potential research opportunities. I am now the tech lead with 5 developers to build this project.</div>
            <div style="margin-top: 20px; font-size: 12pt;">
              <Row :gutter="30">
                <Col :span="12">
                  <p>In this project we used <a href="https://vuejs.org/">Vue.js</a> for front end and Python (Flask) for back end. Besides, data mining service is provided by LibRec through Spark and Hadoop. Until January 2019, we have finished the basic architecture and in process of implementing the fundamental functions.</p>
                  <p style="margin-top: 20px;">This is the first time for me to lead a cross platform data-related project, while my previous production-level leadership experience focused on specific platform, iOS. The first challenge my leadership ran into was the limited, part-time work done by team members. In my team, software developers are all sophomore or senior undergraduates who have their own course schedules and can only do our project as part-time work. The project had been expected to be set up in one semester, which at first overwhelmed some of our developers and even affecting their grades in major courses, decreasing their GPA. <span style="font-weight: bold;">To solve the problem, the lab's professor and me extended our plan of milestone and yielded time of project development to students' coursework. Sooner or later it was proved as a reasonable solution for our team and even encouraged we students to devote in the project, which was beyond our expectation.</span></p>
                  <p style="margin-top: 20px;"><span style="font-weight: bold;">Another challenge we ran into was communication.</span> We team members didn't know each other until the first team meeting --- which somehow obstructed our later communication about the project and triggered misunderstanding of IdeaMan project. Some of our developers didn't follow our conventions and standards about implementation of functions, while adopting their own solutions instead. This problem was solved as soon as we have more chances to exchange our ideas and all team members agree with our common software design rules.</p>
                  <p style="margin-top: 20px;"><span style="font-weight: bold;">Leading a software project is really wonderful experience for me through which I can put my ideas about software architecture, design, innovation and patterns into real-world applications.</span> Through my previous experiences I have had some thoughts about how to lead a software project; thanks to he recommender system lab of Northeastern University, China, which provided me a environment in which I have the opportunity to realize my ideas and make them more solid and robust.</p>
                </Col>
                <Col :span="12">
                  <img :src="images.ideaManIndex" alt="IdeaMan Index Page" style="width: 100%;"/>
                  <img :src="images.ideaManLibrary" alt="IdeaMan Index Page" style="width: 100%; margin-top: 20px;"/>
                </Col>
              </Row>
            </div>
          </Card>
          <Card style="margin-top: 40px;" id="shenma">
            <div slot="title" style="font-size: 12pt;">
              <Row>
                <Col :span="12">
                  <p>Text Classification Model in Shenma Search Knowledge Graph</p>
                </Col>
                <Col :span="12">
                  <p style="text-align: right;">Alibaba Group</p>
                </Col>
              </Row>
            </div>
            <div style="font-size: 12pt;">
              <Row :gutter="30">
                <Col :span="12">
                  <!--<img :src="images.alibabaDraft" alt="First Draft" style="width: 100%;" />-->
                  <img :src="images.alibabaFinal" alt="Final Model" style="width: 100%;" />
                </Col>
                <Col :span="12">
                  <p>My interest in data grew during my internship in Alibaba, a Chinese Tech Giant, where I got a chance of constructing a knowledge graph for Shenma Search with detailed work of training a hierarchical text classification model of users' search queries among 23 first-level categories and 146 second-level categories. I helped to carry out experiments on cutting-edge text classifiers, like ULMFiT, Linear Regression, TextCNN, FastText; and finally chose TextCNN as the model to serve Shenma Search for its high precision on user data.</p>
                  <p style="margin-top: 20px;">This is a special opportunity for me to know about how industry treat AI and machine learning algorithms, how they arrange software development, conduct coding standards and how Alibaba run its business for billions of people in Asia.</p>
                  <p style="margin-top: 20px;">Through this internship experience, Alibaba also taught me how to write robust code and how to collaborate with others in an industry project. For a fresh undergraduate it is really an important experience for preparation as a future software or data engineer.</p>
                </Col>
              </Row>
            </div>
          </Card>
          <Card style="margin-top: 40px;" id="peterbook">
            <div slot="title">
              <Row>
                <Col :span="12">
                  <p>Peterbook: Privacy-concentrated Social Network</p>
                </Col>
                <Col :span="12">
                  <p style="text-align: right;">University of California, San Diego</p>
                </Col>
              </Row>
            </div>
            <div style="font-size: 12pt;">
              <Row :gutter="30">
                <Col :span="12">
                  <p>In Advanced Software Engineering course, my leadership in development of privacy-based social network, Peterbook, was proved as a success, making our software system specially appraised by professor. Until now I still keep in touch with some of my teammates in the project, and we are hoping to have the opportunity to collaborate again in the future; through this experience I also realized more about leadership, colleague inspiration and relationship, enabling me to carry on more complicated leadership work in the future.</p>
                  <p style="margin-top: 20px;">During my life as an exchange undergraduate in UCSD, I once ran into work collision with other team members in CSE 112. In May 2018 there was a chance for our team to conduct an early presentation of our project (also some bonus of score). However, it needed some extra work in that weekend.</p>
                  <p style="margin-top: 20px;">At that time little did I know about coursework of undergraduates there. As the team lead, eager to earn the bonus score, I made the decision by myself to accept the challenge --- which enraged some of my teammates and made the circumstance hard to control. Not until then did I know that UCSD students always have their own time arrangement and I should have asked them about that.</p>
                  <p style="margin-top: 20px;">As a result I was responsible to recover our progress of software project. In the next whole week I sacrificed much of my sleeping time in catching up our progress, designing infrastructure and key components of our social network project. Besides, I had some talk about the my mistake with professor Thomas Powell, who gave me the chance to have a post-mortem speech about our failure in a next session. Thanks to our cooperation later on, we did lead the project to success and most of our team members got A-level final grade. And, through this experience, I have learned to respect every others' time schedule and balance between team democracy and efficiency.</p>
                </Col>
                <Col :span="12">
                  <div class="videoWrapper">
                    <iframe width="560" height="480" src="https://www.youtube.com/embed/RA7DwZiZJxg" frameborder="0" allow="accelerometer; autoplay; encrypted-media; gyroscope; picture-in-picture" allowfullscreen style="width: 100%;"></iframe>
                  </div>
                </Col>
              </Row>
            </div>
          </Card>
          <Card style="margin-top: 40px;" id="mediavault">
            <div slot="title">
              <Row>
                <Col :span="12">
                  <p>MediaVault: Media Storage and Management Website</p>
                </Col>
                <Col :span="12">
                  <p style="text-align: right;"><a href="https://github.com/lalxyy/media-vault-front-end" target="_blank">https://github.com/lalxyy/media-vault-front-end</a></p>
                </Col>
              </Row>
            </div>
            <div style="font-size: 12pt;">
              <Row :gutter="30">
                <Col :span="12">
                  <!--<img src="https://raw.githubusercontent.com/lalxyy/media-vault-back-end/master/Document%20of%20Assignment%203/Diagram%201.png" style="width: 100%;" alt="Diagram 1" />-->
                  <img src="https://raw.githubusercontent.com/lalxyy/media-vault-back-end/master/Document%20of%20Assignment%203/Diagram%202.png" style="width: 100%;" alt="Diagram 2" />
                  <img src="https://raw.githubusercontent.com/lalxyy/media-vault-back-end/master/Document%20of%20Assignment%203/Diagram%203.png" style="width: 100%; margin-top: 20px;" alt="Diagram 3" />
                </Col>
                <Col :span="12">
                  <p>In JSP and Servlet Programming course, as a team lead, we created a Media Vault system; in this project we 2-people team tried Vue.js (like AngularJS) as front end framework, which surprisingly enabled us to reuse much of our code in UI, meanwhile working faster than other teams. For back end, we used Spring Framework to help us reuse codes and split the project into Model-View-Controller structure. This helped a lot when developing the project during the 3 assignments without much modification. For example, we only used 10 lines of code when migrating our storage from assignment 2 XML-based to assignment 3 MySQL-based, thanks to our encapsulation of storage function.</p>
                </Col>
              </Row>
            </div>
            <div style="margin-top: 20px; font-size: 12pt;">
              <p>Some screenshots of my work (using some sample data and pictures) are posted below.</p>
            </div>
            <div style="margin: 20px -10px 0 -10px;">
              <Row :gutter="10">
                <Col :span="12">
                  <img :src="images.mediaList" style="width: 100%;" />
                </Col>
                <Col :span="12">
                  <img :src="images.mediaVault" style="width: 100%;" />
                </Col>
              </Row>
            </div>
          </Card>
          <Card style="margin-top: 40px;" id="vspace">
            <div slot="title">
              <Row>
                <Col :span="12">
                  <p>VSpace: Campus Mobile App for University Students</p>
                </Col>
                <Col :span="12">
                  <p style="text-align: right;">Obisoft Co. Ltd., Shenyang, Liaoning, China</p>
                </Col>
              </Row>
            </div>
            <div style="font-size: 12pt;">
              <p>Based on my knowledge about several programming languages during high school, I quickly got on Swift and Objective-C, while finishing my first app for Northeastern University students to access campus network more easily and get their information like grades, course schedule and campus news on time, building information connection between the school and students. <span style="font-weight: bold;">It was my first software project, and the first iOS app specially designed for the university, which was later revealed as a small success --- although its design and implementation was really naive --- and inspired me about my software projects later.</span></p>
              <p style="margin-top: 20px;">This app provides both Chinese and English version, and pictures below show the app on iPhone 5S in September 2015.</p>
            </div>
            <div style="margin: 20px 10% 0 10%;">
              <Row :gutter="80">
                <Col :span="8">
                  <img :src="images.vspaceIndex" style="width: 100%;" alt="VSpace Index Page" />
                </Col>
                <Col :span="8">
                  <img :src="images.vspaceSide" style="width: 100%;" alt="VSpace Side Page" />
                </Col>
                <Col :span="8">
                  <img :src="images.vspaceLogin" style="width: 100%;" alt="VSpace Login Page" />
                </Col>
              </Row>
            </div>
          </Card>
        </div>
      </Content>
      <Footer>
        <p style="font-size: 12pt;">Ang (Carl) Li, 2019.</p>
      </Footer>
    </Layout>
  </div>
</template>

<script>
  import IdeaManIndex from '@/assets/ideaman_index.jpeg'
  import IdeaManLibrary from '@/assets/ideaman_lib.jpeg'
  import MyPhoto from '@/assets/my_photo.jpg'
  import FirstDraft from '@/assets/first_draft.jpeg'
  import FinalModel from '@/assets/final.jpeg'
  import VSpace1 from '@/assets/vspace_index.png'
  import VSpace2 from  '@/assets/vspace_side.jpg'
  import VSpace3 from '@/assets/vspace_login.jpg'
  import MediaPic from '@/assets/media_vault.png'
  import MediaL from '@/assets/media_list.png'

  export default {
    name: 'app',
    data() {
      return {
        abstract: '',
        images: {
          ideaManIndex: IdeaManIndex,
          ideaManLibrary: IdeaManLibrary,
          myPhoto: MyPhoto,
          alibabaDraft: FirstDraft,
          alibabaFinal: FinalModel,
          vspaceIndex: VSpace1,
          vspaceSide: VSpace2,
          vspaceLogin: VSpace3,
          mediaVault: MediaPic,
          mediaList: MediaL
        }
      }
    },
  }
</script>

<style scoped>
  #app {
    font-size: 12pt;
  }

  .videoWrapper {
    position: relative;
    padding-bottom: 56.25%; /* 16:9 */
    padding-top: 25px;
    height: 0;
  }

  .videoWrapper iframe {
    position: absolute;
    top: 0;
    left: 0;
    width: 100%;
    height: 100%;
  }
</style>
