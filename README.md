# JStarCraft NLP

****

[![License](https://img.shields.io/badge/license-Apache%202-4EB1BA.svg)](https://www.apache.org/licenses/LICENSE-2.0.html)
[![Total lines](https://tokei.rs/b1/github/HongZhaoHua/jstarcraft-nlp?category=lines)](https://tokei.rs/b1/github/HongZhaoHua/jstarcraft-nlp?category=lines)

希望路过的同学,顺手给JStarCraft框架点个Star,算是对作者的一种鼓励吧!

****

## 目录

* [介绍](#介绍)
* [特性](#特性)
* [安装](#安装)
    * [安装JStarCraft Core框架](#安装JStarCraft-Core框架)
    * [安装JStarCraft AI框架](#安装JStarCraft-AI框架)
    * [安装JStarCraft NLP引擎](#安装JStarCraft-NLP引擎)
* [使用](#使用)
    * [设置依赖](#设置依赖)
    * [配置第三方框架](#配置第三方框架)
        * [配置Ansj](#配置Ansj)
        * [配置Stanford CoreNLP](#配置Stanford-CoreNLP)
        * [配置HanLP](#配置HanLP)
        * [配置IK](#配置IK)
        * [配置Jcseg](#配置Jcseg)
        * [配置jieba](#配置jieba)
        * [配置MMSEG](#配置MMSEG)
        * [配置MYNLP](#配置MYNLP)
        * [配置THULAC](#配置THULAC)
        * [配置word](#配置word)
    * 分词
    * 词性识别
* [架构](#架构)
* [概念](#概念)
    * [信息熵](#信息熵)
    * [互信息](#互信息)
* [示例](#示例)
* [对比](#对比)
* [版本](#版本)
* [参考](#参考)
    * [词性标注集](#词性标注集)
* [协议](#协议)
* [作者](#作者)
* [致谢](#致谢)

****

## 介绍

**JStarCraft NLP是一个面向自然语言处理领域的轻量级引擎.遵循Apache 2.0协议.**

专注于解决自然语言处理领域的几个核心问题:
* 词法分析
* 句法分析
* 语义分析
* 信息抽取
* 文本聚类
* 文本分类

涵盖了多种自然语言处理算法,整合了多个自然语言处理框架.为相关领域的研发人员提供提供满足工业级别场景要求的通用设计与参考实现,普及自然语言处理在Java领域的应用.

****

## 特性

* 1.文本相关性
    * 词语相关性
    * 短语相关性
    * 句子相关性
    * 文档相关性
* 2.文本哈希
    * 局部敏感哈希
    * 布隆过滤器
* 3.词法分析(Lexical Analysis)
    * 分词
    * 词性标注
* 4.句法分析(Sentence Analysis)
    * 句法结构分析
    * 依存关系分析
* 5.语义分析(Semantic Analysis)
* 6.信息抽取(Information Extraction)
    * 实体抽取(Entity Extraction)
    * 关系抽取(Relation Extraction)
    * 事件抽取(Event Extraction)
    * 语言检测(Language Detection)
* 7.文本聚类
* 8.文本分类
* 9.兼容Lucene,Solr,ElasticSearch
* 10.整合第三方框架
    * Ansj
    * Stanford CoreNLP
    * HanLP
    * IK
    * Jcseg
    * jieba
    * MMSEG
    * MYNLP
    * THULAC
    * word

****

## 安装

JStarCraft RNS要求使用者具备以下环境:
* JDK 8或者以上
* Maven 3

#### 安装JStarCraft-Core框架

```shell
git clone https://github.com/HongZhaoHua/jstarcraft-core.git

mvn install -Dmaven.test.skip=true
```

#### 安装JStarCraft-AI框架

```shell
git clone https://github.com/HongZhaoHua/jstarcraft-ai.git

mvn install -Dmaven.test.skip=true
```

####  安装JStarCraft-NLP引擎

```shell
git clone https://github.com/HongZhaoHua/jstarcraft-nlp.git

mvn install -Dmaven.test.skip=true
```

****

## 使用

#### 设置依赖

* 设置Maven依赖

```maven
<dependency>
    <groupId>com.jstarcraft</groupId>
    <artifactId>nlp</artifactId>
    <version>1.0</version>
</dependency>
```

* 设置Gradle依赖

```gradle
compile group: 'com.jstarcraft', name: 'nlp', version: '1.0'
```

#### 配置第三方框架

###### 配置Ansj

| 名称 | 功能 | 默认值 |
| :----: | :----: | :----: |
| 名称 | 功能 | 默认值 |

###### 配置Stanford-CoreNLP

| 名称 | 功能 | 默认值 |
| :----: | :----: | :----: |
| 名称 | 功能 | 默认值 |

###### 配置HanLP

| 名称 | 功能 | 默认值 |
| :----: | :----: | :----: |
| 名称 | 功能 | 默认值 |

###### 配置IK

| 名称 | 功能 | 默认值 |
| :----: | :----: | :----: |
| 名称 | 功能 | 默认值 |

###### 配置Jcseg

| 名称 | 功能 | 默认值 |
| :----: | :----: | :----: |
| 名称 | 功能 | 默认值 |

###### 配置jieba

| 名称 | 功能 | 默认值 |
| :----: | :----: | :----: |
| 名称 | 功能 | 默认值 |

###### 配置MMSEG

| 名称 | 功能 | 默认值 |
| :----: | :----: | :----: |
| 名称 | 功能 | 默认值 |

###### 配置MYNLP

| 名称 | 功能 | 默认值 |
| :----: | :----: | :----: |
| 名称 | 功能 | 默认值 |

###### 配置THULAC

| 名称 | 功能 | 默认值 |
| :----: | :----: | :----: |
| 名称 | 功能 | 默认值 |

###### 配置word

| 名称 | 功能 | 默认值 |
| :----: | :----: | :----: |
| 名称 | 功能 | 默认值 |

****

## 架构

****

## 概念

#### 信息熵

**信息熵(Information Entropy)**是指某个片段外部搭配的丰富程度;

#### 互信息

**互信息(Mutual Information)**是指某个片段内部搭配的固定程度;

****

## 示例

****

## 对比

****

## 版本

****

## 参考

#### 词性标注集

| 代码 | 名称 | 词类 | 说明 |
| :----: | :----: | :----: | :----: |
| A | 形容词 | 实词 | 取英语形容词adjective的第1个字母 |
| C | 连词 | 虚词 | 取英语连词conjunction的第1个字母 |
| D | 副词 | 虚词 | 取英语副词adverb的第2个字母 |
| E | 叹词 | 虚词 | 取英语叹词exclamation的第1个字母 |
| M | 数词 | 实词 | 取英语数词numeral的第3个字母 |
| N | 名词 | 实词 | 取英语名词noun的第1个字母 |
| O | 拟声词 | 虚词 | 取英语拟声词onomatopoeia的第1个字母 |
| P | 介词 | 虚词 | 取英语拟声词onomatopoeia的第1个字母 |
| Q | 量词 | 实词 | 取英语量词quantity的第1个字母 |
| R | 代词 | 实词 | 取英语代词pronoun的第2个字母 |
| T | 冠词 | 虚词 | 取英语冠词article的第3个字母 |
| U | 助词 | 虚词 | 取英语助词auxiliary的第2个字母 |
| V | 动词 | 实词 | 取英语动词verb的第1个字母 |
| W | 标点符号 |  |  |
| X | 未知 |  |  |

****

## 协议

JStarCraft NLP遵循[Apache 2.0协议](https://www.apache.org/licenses/LICENSE-2.0.html),一切以其为基础的衍生作品均属于衍生作品的作者.

****

## 作者

| 作者 | 洪钊桦 |
| :----: | :----: |
| E-mail | 110399057@qq.com, jstarcraft@gmail.com |

****

## 致谢

****

