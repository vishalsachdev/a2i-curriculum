# Learning Platform Evaluation

> **Note:** Platform selections would be finalized upon program approval based on institutional resources, existing partnerships, and technical requirements. This document provides a framework for evaluation, not committed platform decisions.

## Requirements Analysis

### Essential Platform Capabilities

The proposed A²I program would require platforms that support:

#### 1. Course Structure & Content Delivery
- Organized course modules with clear progression
- Video hosting and streaming
- Document and resource management
- Mobile-responsive interface
- Offline content access capability

#### 2. Assessment & Feedback
- Multiple assignment types (written, code, multimedia)
- Peer review workflows
- Automated grading for objective assessments
- Rubric-based grading for subjective work
- Oral viva (video assessment) capability
- Grade management and reporting

#### 3. Communication & Collaboration
- Discussion forums with threading
- Direct messaging
- Announcement systems
- Group workspaces
- Video conferencing integration

#### 4. Learning Analytics
- Student progress tracking
- Engagement metrics
- Predictive analytics for intervention
- Learning outcome assessment
- Reporting dashboards

#### 5. Technical Lab Environments
- Cloud computing resources (compute, storage)
- Big data processing tools
- AI/ML development environments
- Collaborative coding environments
- Version control integration

#### 6. Integration & APIs
- Single sign-on (SSO)
- Grade passback
- Calendar integration
- External tool integration (LTI standard)
- Analytics and reporting APIs

## Platform Options Considered

### Canvas LMS

**Overview:**
Canvas is a widely-adopted learning management system used by many higher education institutions.

#### Strengths for A²I Program
- **Institutional Compatibility**: Many universities already license Canvas
- **Robust Assessment Tools**: Supports diverse assignment types including SpeedGrader for video assessments
- **Strong Mobile App**: Well-designed mobile experience for students
- **Peer Review Capability**: Built-in workflows for peer feedback
- **Extensive Integrations**: LTI support for external tools
- **Discussion Forums**: Threaded discussions with rich text and media
- **API Access**: Comprehensive APIs for custom integrations

#### Limitations
- **Video Content**: Not optimized for hosting large video libraries (would need supplementary platform)
- **Learning Analytics**: Basic built-in analytics; advanced features require additional tools
- **Content Authoring**: Limited compared to specialized e-learning platforms
- **AI Integration**: Would require custom development or third-party tools

#### Cost Considerations
- Typically licensed at institutional level
- Per-student pricing if not institutionally licensed: ~$5-15 per student
- Additional costs for premium features or integrations

#### Suitability for A²I: **High**
Canvas could serve as the primary LMS for course structure, assessments, and grade management, supplemented by other platforms for video content and technical labs.

---

### Coursera

**Overview:**
Coursera is a leading MOOC platform with extensive corporate and university partnerships.

#### Strengths for Asynchronous Delivery
- **Optimized Video Experience**: Excellent video player with speed control, transcripts, mobile optimization
- **Scalable Content Delivery**: CDN infrastructure for global access
- **Learner Experience**: Polished, intuitive interface refined over millions of users
- **Assessment Variety**: Auto-graded quizzes, programming assignments, peer review
- **Credential Management**: Integrated certificates and degree programs
- **Global Reach**: Infrastructure proven for international delivery
- **Content Authoring Tools**: Sophisticated tools for creating engaging content

#### Limitations
- **Customization**: Less flexible than open-source LMS for institutional branding
- **Cost at Scale**: Potentially expensive for large degree programs
- **Integration**: May require complex integration with institutional systems
- **Control**: Less institutional control over platform evolution
- **Discussion Forums**: Basic compared to dedicated LMS platforms

#### Partnership Requirements
- Institutional partnership agreement
- Revenue sharing or licensing fees
- Content must meet Coursera quality standards
- Potential restrictions on content reuse

#### Cost Considerations
- Partnership models vary: licensing fees or revenue sharing
- Typical degree program fees: $15,000-25,000 total per student
- Institution may receive 50-70% of revenue
- Coursera handles marketing, support, platform costs

#### Suitability for A²I: **Medium-High**
Coursera could handle primary content delivery and student experience, but would require supplementary tools for technical labs and potentially institutional LMS for official records.

---

### Google Cloud Platform (GCP)

**Overview:**
Google Cloud Platform provides cloud computing services including compute, storage, big data, and AI/ML tools.

#### Strengths for Technical Labs
- **Comprehensive AI/ML Tools**: Vertex AI, AutoML, pre-trained models
- **Big Data Processing**: BigQuery, Dataflow, Dataproc
- **Analytics & Visualization**: Looker, Data Studio
- **Development Environments**: Cloud Shell, Jupyter notebooks, Colab
- **Real-World Tools**: Students learn platforms used in industry
- **Scalable Resources**: Allocate compute as needed
- **Security & Governance**: Enterprise-grade security and compliance

#### Educational Benefits
- **Google Cloud Education Grants**: Significant credits available for academic programs
- **Qwiklabs Integration**: Pre-built lab exercises and learning paths
- **Professional Credentials**: Students can pursue Google Cloud certifications
- **Industry Alignment**: Skills directly transferable to workplace

#### Limitations
- **Learning Curve**: Complexity may challenge students without technical backgrounds
- **Cost Management**: Requires careful monitoring to control costs
- **Not a Learning Platform**: Requires LMS for course structure and content delivery
- **Support Requirements**: Students need technical support for cloud issues

#### Cost Considerations
- **Education Grants**: Google typically provides $50-100 per student in credits
- **Ongoing Costs**: ~$20-50 per student annually beyond grants
- **Faculty Development**: Training costs for instructors
- **Technical Support**: Staff time for troubleshooting

#### Suitability for A²I: **High**
GCP is well-suited for technical lab requirements and aligns with program focus on business applications of AI. Should be supplemented with learning platform for course delivery.

---

### GitHub

**Overview:**
GitHub is a development platform providing version control, collaboration, and code hosting.

#### Role in Portfolio Assessment
- **Version Control**: Students learn professional development practices
- **Project Documentation**: README files, wikis, and documentation
- **Portfolio Building**: Public repositories showcase student work
- **Collaboration**: Pull requests, code review, issue tracking
- **GitHub Classroom**: Tools specifically designed for education
- **GitHub Pages**: Students can host project websites

#### Educational Benefits
- **Industry Standard**: Essential tool for technical professionals
- **GitHub Education**: Free access to premium features for students and educators
- **Resume Value**: Public portfolio visible to employers
- **Collaboration Skills**: Learn distributed teamwork practices
- **Open Source**: Can contribute to public projects

#### Limitations
- **Not an LMS**: Requires separate platform for course structure
- **Learning Curve**: Git can be challenging for non-technical students
- **Limited Assessment Tools**: Not designed for grading
- **Privacy Considerations**: Students may prefer private repositories

#### Cost Considerations
- **GitHub Education**: Free for academic institutions
- **GitHub Team**: $4/user/month if additional features needed
- **GitHub Enterprise**: $21/user/month for advanced features (likely unnecessary)

#### Suitability for A²I: **High**
GitHub is ideal for portfolio development and project-based learning. Essential complement to primary LMS, not a replacement.

---

### Alternative Platforms Considered

#### Moodle
- **Pros**: Open-source, highly customizable, no licensing fees
- **Cons**: Requires technical resources for hosting and maintenance, dated user interface
- **Verdict**: Viable if institutional resources available for support

#### edX (Open edX)
- **Pros**: Open-source MOOC platform, similar to Coursera
- **Cons**: Requires significant technical resources to host and maintain
- **Verdict**: Consider only if seeking fully self-hosted solution

#### AWS Academy
- **Pros**: Alternative to GCP with similar capabilities, AWS Educate program
- **Cons**: Slightly less aligned with program focus (GCP stronger in AI/ML tools)
- **Verdict**: Acceptable alternative if institutional preference or existing partnership

#### Microsoft Azure
- **Pros**: Azure for Students program, comprehensive AI services
- **Cons**: Interface complexity, less established in academic data science
- **Verdict**: Acceptable alternative with appropriate faculty expertise

## Recommended Multi-Platform Approach

Based on requirements analysis and platform evaluation, a **multi-platform integration strategy** is recommended:

### Recommended Architecture

```
Primary Course Management: Canvas LMS or institutional equivalent
     ↓
Content Delivery: Coursera or custom video platform
     ↓
Technical Labs: Google Cloud Platform
     ↓
Portfolio & Code: GitHub
     ↓
Collaboration: Slack/Teams or Canvas discussions
     ↓
AI Support: Custom or vendor solution (e.g., ChatGPT API integration)
```

### Platform Roles

1. **Canvas (or institutional LMS)**: 
   - Official course structure and navigation
   - Assessment submission and grading
   - Grade book and official records
   - Learning pod organization
   - Calendar and due dates
   - Oral viva assessments

2. **Coursera (or alternative video platform)**:
   - Instructional video content
   - Auto-graded knowledge checks
   - Searchable transcripts
   - Mobile-optimized viewing
   - Content analytics

3. **Google Cloud Platform**:
   - Hands-on technical exercises
   - Data analysis projects
   - AI model development
   - Real-world tooling practice

4. **GitHub**:
   - Code repository for projects
   - Portfolio documentation
   - Peer code review
   - Version control practice

5. **Communication Platform**:
   - Learning pod communication
   - Quick questions and peer support
   - Community building
   - Announcements

### Integration Points

**Canvas ↔ Coursera**:
- LTI integration for seamless access
- Grade passback for Coursera assessments
- Single sign-on for unified experience

**Canvas ↔ GCP**:
- Lab assignment links in Canvas
- Submission of GCP project artifacts via Canvas
- Usage monitoring and cost tracking

**Canvas ↔ GitHub**:
- Repository submission via Canvas assignments
- GitHub Classroom integration for assignment distribution
- Portfolio reviews conducted in Canvas with GitHub links

**Analytics Integration**:
- Aggregate data from all platforms for comprehensive learning analytics
- Early warning systems for student struggling across platforms
- Unified dashboard for faculty and advisors

## Implementation Considerations

### Technical Requirements

**Infrastructure:**
- Reliable internet connectivity for faculty and students
- Technical support team for platform issues
- Integration development resources (if building custom connections)
- Data warehouse for consolidated analytics (optional but recommended)

**Security & Privacy:**
- FERPA-compliant data handling
- Secure authentication (SSO preferred)
- Data protection agreements with vendors
- Student data privacy policies

**Accessibility:**
- WCAG 2.1 AA compliance across all platforms
- Closed captioning for all video content
- Screen reader compatibility
- Keyboard navigation support

### Faculty Development Needs

**Training Topics:**
- Platform-specific functionality for each tool
- Online pedagogy and engagement strategies
- Creating accessible content
- Using learning analytics effectively
- Integrating AI support tools
- Managing cloud computing resources
- Facilitating asynchronous discussions

**Ongoing Support:**
- Instructional design consultation
- Technical troubleshooting support
- Peer learning community
- Regular faculty development workshops
- Resource library and documentation

### Student Onboarding

**Orientation Modules:**
- Platform navigation tutorials for each tool
- Technical requirements and setup
- Learning pod guidelines
- Communication expectations
- Academic integrity policies
- Time management for asynchronous learning
- How to get help

**Technical Support:**
- Help desk for platform issues
- Setup guides and FAQs
- Video tutorials
- Live troubleshooting sessions (optional)
- Peer support community

## Risk Assessment

### Platform Stability Risks
- **Risk**: Platform outage during critical period (e.g., exam)
- **Mitigation**: Redundant submission options, flexible deadlines, service level agreements with vendors

### Integration Complexity
- **Risk**: Platform integrations fail or require excessive maintenance
- **Mitigation**: Start with manual workflows, automate incrementally, maintain fallback procedures

### Cost Escalation
- **Risk**: Platform costs exceed budget as program scales
- **Mitigation**: Negotiate volume pricing, monitor usage carefully, evaluate alternatives annually

### Faculty Resistance
- **Risk**: Faculty struggle with platform complexity or resist online teaching
- **Mitigation**: Comprehensive training, instructional design support, showcase early successes

### Student Technology Access
- **Risk**: Students lack reliable internet, devices, or technical skills
- **Mitigation**: Mobile-first design, offline capabilities, technical requirement transparency, loaner programs

## Alternative Scenarios

### Scenario 1: Minimum Viable Platform Stack
If resources are constrained:
- **Canvas only** (or institutional LMS)
- **GCP for labs** (using education grants)
- **GitHub** (free for education)
- **Embedded videos** in Canvas (no Coursera)
- **Canvas discussions** (no separate chat platform)

**Tradeoffs**: Less polished video experience, more manual integration, higher faculty workload

### Scenario 2: Premium Platform Stack
If resources are abundant:
- **Coursera** for full content delivery and student experience
- **Canvas** for institutional integration and official records
- **GCP** with generous budget for advanced AI labs
- **GitHub Enterprise** for advanced features
- **Slack** or **Teams** for communication
- **Custom AI learning assistant** development
- **Comprehensive learning analytics platform**

**Benefits**: Superior student experience, powerful analytics, competitive differentiation

### Scenario 3: Fully Open-Source
If institutional philosophy favors open-source:
- **Open edX** or **Moodle** for LMS
- **Kaltura** or **Panopto** for video hosting
- **JupyterHub** for coding labs (with GCP/AWS backend)
- **GitHub** for code repositories
- **Mattermost** or **Rocket.Chat** for communication

**Tradeoffs**: Higher technical support burden, potentially less polished UX, full control

## Recommendation Summary

For the initial program launch, recommend:

### Phase 1 (Years 1-2): Proven Platform Stack
- **Canvas**: Primary LMS (likely already licensed by institution)
- **Coursera**: Video content delivery (if partnership can be established) OR custom video hosting in Canvas
- **GCP**: Technical labs (using education grants)
- **GitHub**: Code portfolios (free for education)
- **Canvas Discussions**: Communication (no additional tool)

**Rationale**: Proven platforms, manageable integration complexity, leverages institutional resources

### Phase 2 (Years 3+): Enhanced Platform Stack
Based on program growth and feedback:
- Add dedicated communication platform (Slack/Teams)
- Develop custom AI learning assistant
- Implement comprehensive learning analytics
- Consider additional platforms based on emerging needs

**Rationale**: Incrementally enhance based on demonstrated need and available resources

## Detailed Integration Specifications

Upon program approval, the following technical specifications would be developed:

- Platform architecture diagrams
- API integration specifications
- Data flow and security protocols
- Authentication and authorization schemes
- Disaster recovery and backup procedures
- Monitoring and alerting systems
- Scalability plans
- Detailed cost projections by platform

*These specifications are available upon request as part of implementation planning*

---

**Related Documents:**
- [Delivery Options](./delivery-options.md) - Overall delivery model recommendation
- [Curriculum Overview](../curriculum/overview.md) - Program structure informing platform needs
- [Pedagogical Approach](../pedagogy/README.md) - Teaching models requiring platform support
