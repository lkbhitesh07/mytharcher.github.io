---
layout: post
title: 一个团队主页的诞生——Web 设计入门级参考
category: thinking
---

> 友情提示：这是一篇硬广，当然也有干货。

在我入行之前几年，还没有前端这个职业，而我做的事情其实被称作的是“美工”。那段在学校的时间里，我的职责其实更像设计师，构思界面要放置的信息，确定整体风格色调，排列布局，再把实际细节实现成 HTML+CSS 的代码交给后端。不过在入行转职的时候，最终选择的路线是工程师，原因是毕竟没有大量的美学基础，而且对代码更有兴趣一些，也有一定的专业基础。

今年从自由职业转为团队建设，为了给团队包装一个品牌，再次捡起“美工”这项被放弃已久的手艺，从开始设计到最终上线折腾了两个星期，虽然最后也就很简单的一个页面，但其中的过程很想分享给准备走上 Web 设计路线的新人们，所以顺便把整个过程记录下来。不过这毕竟是我这种业余选手的拙作，所有的思考也都是没有经过任何专业培训的自我理解，专业的设计师们请轻喷。

品牌创意
----------

不能否认的是，新的团队品牌是先有域名，才有其他。使用 **Rogue** 这个名词来源于星球大战的电影《Rogue One》，是一个游击小队通过自身努力对大战局做出很大影响的故事。

首先进入的流程就是品牌形象最重要的环节——VI，VI 之中大家认知最普遍的也就是 Logo 设计（虽然 VI 之中还有很多其他内涵，但这里我就不做过多不专业的扩展了）。

Logo 的设计我个人只知道有一些常（di）见（ji）的方法，比如直接简单硬堆文字，字体颜色变形，团队吉祥物和意象融合等。

我们暂时还没有团队吉祥物，所以这条路完全不通。不过由于 Rogue 这个单词其实比较简单，直接硬堆文字并不是不可以，但找一个合适的字体产生一定的辨识度并不容易。所以我想还是希望找一些容易产生联想的意象进行融合可能会更好。

可能是我的想象力被长期的代码逻辑式的思维限制住了并不够丰富，意象的构思占据了我很大一部分时间。从最后选中的结果反过来看是这样的思考路径：Rogue 是一个游击队，在意象上和军队有关，很容易就想到每个士兵最基本的武器——枪，但整个枪的图形结构太复杂，要表现出来并且得到清楚的视觉传达不容易，功力不够的话很容易成为一个失败的案例。再往下分解和尝试后，我最终选择了枪上面的瞄准镜这个比较简单又有一定代表性的部件，作为图案的核心意象。瞄准镜象征着精准的解决目标，也符合我们整个团队帮助客户高效解决问题的定位。

有了这个基础思路，立即着手做了一些图案设计。其中还要考虑和团队名称文字的结合，瞄准镜通常是一个圆圈，正好可以结合字母 O 来进行融合，或者反过来选择合适的字体来进行风格匹配。大多数字体对字母 O 的表现都大致是椭圆形，而不是正圆，从这个考虑上我就筛掉了很多。在翻着 [Google web font](https://fonts.google.com/) 和系统自带的字体册纠结了很久之后，我最终在字体册里找到一个和图形比较容易匹配的字体——SchoolHouse Print。这个字体的线条简洁直白，但不像其他很多边缘带尖角的字体那么强硬，圆角边缘会显得更加亲和。

另一方面针对瞄准镜的图案进行了尽可能的简化，仅仅保留外围四根很短的刻度线和中心圆点，也是为了配合字体替代 O 字母。再为了和普通的瞄准镜图案有所区别，我又将其旋转了一个较小的角度，有点歪打正着的意味，也符合 Rogue 的气质。

<figure>
    <img src="http://www.rogue.group/assets/img/logo.png" alt="ROGUE" />
</figure>

这样整体的 Logo 图案和核心 VI 就确定下来，在空间足够的地方就应用带文字的融合图案，而紧凑的地方单独使用瞄准镜图案就可以满足不同场景的需求。

信息架构
----------

接下来的核心就是要确定希望如何向受众说明白我们想表达内容。我还希望在一个页面内就能尽量说完大部分内容，一是现在大家的时间都很宝贵，很多受众不一定会仔细的去“探索”那些被“藏起来”的内容；二是要做的越多，时间成本也就越高，我们暂时还不是一个多大价值的品牌，还有更多更重要的事情要去做。

即使从流行的角度，很多新一代的官网主页设计也都非常简洁，大多控制在一个网页之内。我也比较认同这种方式，不说废话。

那么从信息传达上来讲，下面的这些问题就构成了基本的大纲：

* 我们是谁？Who we are
* 我们能做什么？What we do
* 我们怎么做？How we do
* 为什么找我们？Why us
* 如何联系我们？Where are we

基本上就是 4W+1H 的结构，能在最短的时间内回答出这些问题就已经足够了。对应到具体的内容上也就按这个结构每个部分留一屏左右的空间来具体说明。

### 我们是谁 -> VI

* 突出展示团队 VI 形象
* 一句话说明我们是干什么的团队
* 团队成员的形象展示

在首屏，最重要的就是给受众一个良好的第一印象，能产生独特记忆的就更好。因为目前来看我们团队做的事情并不那么特殊，很多其他人也在做，所以只有 Logo 和团队形象能有个较大的区别，一句话的标语（slogan）说的也比较朴实，并没有吹的特别高大上。

### 我们能做什么？-> 我们的服务

* 服务内容内容
* 服务的业务场景

第二页要说明我们的服务内容，简单直白最好，这部分能够中规中矩就行。

### 我们怎么做？-> 项目执行的方式

这部分实际上是上一部分服务内容的加深，光告诉受众我们能做什么是不够的，最好还要有说服力的告诉他们我们是怎样去做的。于是我准备在这布置一张流程图，对于潜在客户比较容易理解。

### 为什么找我们？-> 案例展示

当潜在客户知道我们能做什么以及怎样做以后，最有说服力的就是用之前与其他客户合作的案例来说明了。当然不可能展示所有曾经的案例，所以也可以有几个简单的统计数字，这也是国外一些网站常见的做法。一般还会放一块客户评价的内容，但这部分需要找之前的客户帮忙提供，所以只能在日后再添加。

### 如何联系我们？-> 联系方式

这个部分需要提供的是让潜在客户方便的找到我们并进行联系的功能。对于我们这样的技术团队来讲，地址的意义通常不大，尤其是我们很多客户也都不在当地。所以一个留言框和一个用于对外联系的邮箱地址就足够了。

同时最后有一些不是那么重要的信息可以作为页脚一起收尾就行，比如版权等。

素材收集整理与排版
----------

按照上面的信息架构，下一步就要进入内容排版环节。大部分每一页里面的内容基本是标题 + 简短文字 + 图片/功能块的方式，除了服务内容和案例可以比较结构化。于是对于可以结构化的内容部分都使用了一致的栅格布局来排列，其他的图文就是很直白的居中平铺。

排版的过程里，我也借（chao）鉴（xi）了很多类似网站的方式，通过满屏滚动来连接内容，每都使用了独特的背景图片，既是对当前内容主题的烘托，又区分了每一屏的内容结构。

不过找图和 P 图才是整个主页项目过程中花费时间最多的部分，毕竟在这方面不是专业的。尤其是我们团队的那张照片，单把人物扣出来就花了一早上。不过这个过程尤其是案例的部分也是一个很好的总结和整理，不去做根本没想到这些年做了这么多项目，最后也只能挑一些出来整理成我们的作品集。

然后我要强烈安利一个网站 [Pixabay](https://pixabay.com/)，这上面有数以百万计的可以免费使用的高质量商业图片（记不住网址的在谷歌里搜“免费图片”，第一个非广告的结果就是）。要是没有这个网站提供的图片素材，我估计会被自己设计的结果丑哭。当然我也看了很多 [站酷](http://www.zcool.com.cn/) 的案例以及一些国外的设计类站点，激（chao）发（xi）了很多灵（su）感（cai）。

动效、响应式与功能实现
----------

前面的设计都做完了，终于到了我更擅长的用代码实现的部分。

其实这部分也很难在设计软件中表达清楚，尤其是动效。不过由于整体的风格定的比较简洁，也不适合做大量的效果，只是在一些有限区域进行内容展开的时候用到一小部分，而且都是纯 CSS 实现，尽量降低实现的成本，毕竟只是锦上（xuan）添花（ji）的效果。

对于需要团队配合的设计师，我个人建议在做响应式设计的时候尽量给出不同分辨率（设备）下所希望的样式效果。除非是像我这样一个人做的话就可以省略，因为自己完全清楚不同尺寸下应该如何排列各种内容。

另外说说其他两项功能。一个是要在无后端支持的情况下允许客户发送留言到我们的邮箱，这个有很多类似问卷类的服务都可以用，不过我选用了国外一个叫做 [FORMSPREE](https://formspree.io/) 的极简表单数据发送服务，只需写纯 HTML，一行 JS 都不用就可以完成。

还有一个是通过前端字典表做了主要内容的多语言化，保证当我们给国外客户浏览的时候也能够明白我们想表达的内容。这也是这个页面里面唯一用到 JS 的地方。

这样实现这些功能最大的原因其实是低成本，因为完全可以在 Github 免费提供的 Pages 服务上部署网站，无需管理一个服务器，对于这类纯静态展示类的网站，应该没有比这更适合的方案了。尤其我们的案例部分也是使用了 Jekyll 静态生成器来管理，很方便今后随时添加修改。

上线
----------

其实到上线这一步已经没有太多可说的，尤其是选择了 Github Pages 服务，仓库准备好提交推送就好了，唯一需要注意的是在使用自定义域名的时候，如果使用的裸域的 MX 记录作为邮件服务器的指向，那么再使用裸域的 CNAME 指向 Github 会造成 DNS 解析冲突，虽然实际使用不会有太大的问题，但仍需小心。所以我改用了`www`子域名来做正式访问域名的方式，毕竟 A 记录万一 IP 发生变化（虽然几率较小）又得去改一次比较麻烦。

好了，最后其实没什么可说的了，整个过程其实并没有特别厉害的地方，大多中规中矩，只能当做一个想入 Web 设计这一行的新人的练习小作业。因为真正专业的设计师可能并不需要花我这么多时间在这上面，也会比我做的更好。所以整个案子仅供新人们参考。

**最后放出硬广部分：<https://www.rogue.group/>**
