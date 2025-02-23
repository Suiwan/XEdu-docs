# XEdu的设计

## XEdu的定位是什么？

XEdu的全名为OpenXLabEdu，是基于OpenXLab的教育版，也是为中小学AI教育设计的一套完整的学习工具。OpenXLab是上海人工智能实验室开源的AI工具集合。

XEdu核心工具为计算机视觉库MMEdu，加上神经网络库BaseNN和传统机器学习库BaseML，后期规划中会增加OpenDILabEdu和OpenDataLabEdu等，覆盖实验室开源的所有人工智能工具，支持中小学可能涉及到AI技术所有领域。

## 揭秘XEdu

### 1.应用先行，逐层深入

XEdu的核心工具MMEdu内置SOTA模型，让学生把机器学习作为解决问题的有效工具，先应用，再逐步研究背后的原理。就如互联网，不是先讲ISO七层协议，而是先打开浏览器获取信息，打开EMail交流信息，再慢慢走向底层的协议。

XEdu的基础工具BaseDT，则是一个整合了常见数据处理工具的基础库。借助这个库，用一行代码即可完成数据的预处理，让AI应用的代码更加简洁。

### 2.代码最简，部署方便

将AI工具分解为“训练”和“部署”两种核心功能。无论是BaseML、BaseNN还是MMEdu，全部采用一致的语法完成训练、推理和转换、部署。

### 3.兼容并蓄，灵活扩展

虽然语法上做到最简，但是兼容原生工具的各种功能，如BaseNN和BaseML分别保留了Pytorch和Sklearn的功能，MMEdu则保留了OpenMMLab的各种参数，尤其是模型训练的所有常见参数，让学生在不同阶段都可以使用OpenXLab的系列工具进行学习。在不久的将来，用BaseNN可以搭建MMEdu的模型，多个工具形成一个强大的AI工具包，能支撑中小学绝大多数的AI学习。

## 了解XEdu的规划

1.计算机视觉开发库：MMEdu

MMEdu全称为OpenMMLabEdu，是著名的计算机视觉开发工具OpenMMLab的教育版本。 

2.神经网络开发库：BaseNN

BaseNN是神经网络库，能够使用类似Keras的语法搭建神经网络模型。

3.传统机器学习开发库：BaseML

BaseML是传统机器学习库，类似Sklearn，使用了与MMEdu同样的语法。 

4.数据处理工具库：BaseDT

不同的模型对数据有特定的要求，比如LeNet-5是28*28*1，MobileNet是224*224*3。BaseDT集成了这些转换工具。

5.Easy系列工具

一系列方便初学者的小工具，可以在无代码的情况下完成模型的训练、推理、转换和部署，甚至可以搭建一个WebAPI服务器，类似百度AI开放平台。

6.其他规划中的库

规划中的库还有OpenDILabEdu和OpenDataLabEdu，从名称可以看出源自上海人工智能实验室的各种工具。

![](../images/about/xedu_plan.png)

## XEdu的愿景

“接地气，望云端”，开源科创团队期望XEdu是一款适合中小学生入门，同时又能编写出可以“真正运行”的AI代码的人工智能开发工具，让学生能够通过完成各种AI实验，亲历从收集数据到训练深度学习模型的过程，并能够通过训练AI模型、部署智能信息系统的方式，解决生活中的真实问题。
