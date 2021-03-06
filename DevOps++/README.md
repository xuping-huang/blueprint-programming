# DevOps后对团队开发的继续改进

DevOps正在成为软件开发的业界标准。因为越来越多的代码量、越来越短的交付时间，都需要一种更高质量的开发过程。DevOps通过持续集成、持续部署以及可附加的同行评审、代码规范自动审核与自动测试来提高开发质量。

DevOps与敏捷开发模式Scrum的配合，较好的管理了开发团队成员的工作量、工作质量与工作进度，这也是项目的核心三要素。但是DevOps+Scrum的模式仍然对项目中的一些问题没有涉及。

1. 短生命周期与长生命周期的项目没有区分。短周期项目的人员结构比较稳定，成员从项目起始就加入进来，对项目的了解深入。而长周期项目会出现人员的变动，有可能完全替换一批。新人只能通过代码和文档去熟悉了解，但是从代码难以产生对产品的架构了解，而从文档又难以直观了解实现。两者间是脱离的。这必然造成效率与质量的下降，频繁的更换给项目带来的隐患可能会持续很长时间。

2. 缺少对人员能力的更准确全面的评估。工作量，质量与进度是每个成员最重要的指标，但是在一个较长时间运行的项目中，成员的某些特点会对项目后期带来更大的利益，但是目前确无法体现出来。这些特点包括团队协作性，分享精神，自我成长能力。一位团队协作性好的成员可以让团队的气氛更加融洽，运转更加顺畅，但是目前我们只能从其密切接触者获得相对主观的了解，一旦更换项目，大家需要重新认识。具有分享精神的成员能够让新人更快的融入团队，提高团队运转效率，这一特点更是难以发现和传播。而成员的自我成长能力是其自身能否快速适应项目，承担起关键角色的重要指标。当团队领导者无法通过客观的数据综合评估一位成员时，那只能通过经验与传闻来判断，这又对项目经理这方面的能力依赖。

3. 缺少对团队及领导者能力的更全面评估。例如团队抗压力与风险的能力，是否关键岗位上缺少备用人员，因为一个人影响整个项目的交付。项目经理能否及时发现并解决项目中的这些风险。

4. 缺少对长远利益行为的正向激励。例如鼓励成员更多的将自己对项目的经验体会分享出来，帮助别人少走弯路。鼓励开发合适的工具，帮助团队提高效率。

5. 缺乏造血机制，新人加入团队后往往是自行摸索。老带新已经是业界最好的方法，但是这又受到个人特性以及项目进度压力的多重影响。

##	基于以上的问题，提出下面对项目过程改进的几个方面。

### 达到架构穿透效果的文档体系。

当软件交付时，会有一个完整的功能模型，由软件的各个功能点组成。而软件的架构会分为业务架构与技术架构。这两个架构是与功能模型交错在一起的。

例如安全与认证技术架构，除了作为中间件的安全认证模块，还需要登录界面以及分布在各功能页面前后端的Token存储与安全检查机制作为配合。现有的文档体系只能从某一个角度进行描述，确无法带给团队成员具有穿透效果的体验。例如，对于一个开发人员，如果在查看项目的安全与认证技术架构文档时，能够看到技术架构落地到功能模块的哪个位置，并能够穿透看到当前的实现代码，那么对理解和维护架构会有相当的正向影响。

而业务架构具有同样的特点，例如一个资源分配的业务，除了在管理端的资源分配功能外，在相应的业务功能还会有资源分配调整的影响，这些同样可以与功能模结合，来理解业务。

穿透应当不止局限于现有信息保存，应当能够保持历史记录，

###	多模态可留存的分享体系以及对分享的正向激励机制。

DevOps中的分享目前可以在Wiki和代码同行评审中体现，除此之外的分享机制更多依赖于团队成员间的私下交流或者不定期的内部培训。除了Wiki之外，其余的分享机制是无法进行留存的，即使是Wiki，因为没有精心的组织，效果完全因人而异。

我们希望的分享是基于前述的功能架构、技术架构和业务架构进行精心规划的，能够留存的，并为项目的运作带来足够帮助的分享机制。分享应当渗透在项目运作的每个角落。

例如对于一位开发人员，当他为某一业务流程进行开发时，可以在业务架构中创建或修改相应的业务条目，将开发中遇到的问题和解决方案的选择记录下来，这些并不合适作为代码注释；对于技术架构也同样如此。此外对于某一次系统缺陷的调试与修复也可以附加到相应的技术架构中。因为类似的错误可能在不同模块中重写，基于技术架构留存的这些知识点，为以后处理或避免类似问题会带来良好的益处。

不同的项目角色应当有各自符合其承担责任的分享内容。例如架构师应当成为技术架构分享的主要贡献者，而产品经理应当成为业务架构分享的主要贡献者。

每个人的分享都应当留存下各自的标记，并有公平合理的机制为每个人的分享进行评分。作为对个人能力综合评价的一个重要补充。

可以说所有除直接开发工作之外的，对项目团队运作有利的工作都应当被看作分享的一种。包括项目经验的留存，制作的培训资料、视频，制作的考试，提效工具的开发，岗位成长路线图制作等等。

###	全面的团队穿透性评估体系。
###	对个人的全面评分机制。
###	团队造血能力
###	团队及个人的效率改进推动机制
###	团队开发过程改进的推动机制
###	团队一致性保证机制
