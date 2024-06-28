---
layout: post
title: AI Engineering with Azure
subtitle: Learning how to use AI Engineering on Azure
categories: AI
tags: [Azure, Ai Engineering, Generative Ai]
---

## AI ENGINEERING ON AZURE
### Get started with Azure AI Services
1. Define artificial intelligence:

Artificial Intelligence (AI) is increasingly prevalent in the software applications we use every day; including digital assistants in our homes and cellphones, automotive technology in the vehicles that take us to work, and smart productivity applications that help us do our jobs when we get there.

we tend to think of AI as software that exhibits one or more human-like capabilities, such as:

Visual perception - The ability to use computer vision capabilities to accept, interpret, and process input from images, video streams, and live cameras.

Text analysis and conversation - The ability to use natural language processing (NLP) to not only "read", but also generate realistic responses and extract semantic meaning from text.

Speech - The ability to recognize speech as input and synthesize spoken output. The combination of speech capabilities together with the ability to apply NLP analysis of text enables a form of human-compute interaction that's become known as conversational AI, in which users can interact with AI agents (usually referred to as bots) in much the same way they would with another human.

Decision making - The ability to use past experience and learned correlations to assess situations and take appropriate actions. For example, recognizing anomalies in sensor readings and taking automated action to prevent failure or system damage.

2. Understand AI-related terms:

   There are several related terms that people use when talking about artificial intelligence, so it's useful to have clear definitions for each.

   i. Data Science

   ii. Machine Learning

   iii. Artificial intelligent.

3. Understand considerations for AI Engineers

   Increasingly, software solutions include AI features; so software engineers need to know how to integrate AI capabilities into their applications and services.

   The advances made in machine learning, together with the increased availability of large volumes of data and powerful compute on which to process it and train predictive models, has led to the availability of prepackaged software services that encapsulate AI capabilities. Software engineers can take advantage of these services to create applications and agents that use the underlying AI functionality, using them as building blocks to create intelligent solutions.

4. Understand considerations for responsible AI

   i. Reliability and safety

   ii. fairness

   iii. Privacy and security

   iv. Inclusiveness

   v. Transparency

   vi. Accountability

5. Understand capabilities of Azure Machine Learning:

   Azure Machine Learning provides the following features and capabilities:

  Automated machine learning	This feature enables non-experts to quickly create an effective machine learning model from data.

  Azure Machine Learning designer	A graphical interface enabling no-code development of machine learning solutions.

  Data and compute management	Cloud-based data storage and compute resources that professional data scientists can use to run data experiment code at scale.

  Pipelines	Data scientists, software engineers, and IT operations professionals can define pipelines to orchestrate model training, deployment, and management tasks.

6. Understand capabilities of Azure AI Services:

   Azure AI Services are cloud-based services that encapsulate AI capabilities. Rather than a single product, you should think of Azure AI Services as a set of individual services that you can use as building blocks to compose sophisticated, intelligent applications.

7. Understand capabilities of the Azure OpenAI Service:

   Generative AI is a relatively new and quickly progressing field of AI focused on AI models that generate content. Content that these models generate can be in the form of text, images, code or more, and in a way that almost feels like interacting with a real person in a real conversation. Generative AI models depend on large language models (LLMs) based on the transformer architecture that evolved from years of machine learning progress. Generative AI models are often queried with natural language prompts, and return an impressively accurate response when prompted correctly.

8. Understand capabilities of Azure Cognitive Search

   Searching for information is a common requirement in many applications, from dedicated search engine web sites to mobile apps that can find context-appropriate information based on where you are and what you want to accomplish.

### Develop decision support solutions with Azure AI Services 
1. Overview of text moderation:

When you're using machine-assisted content moderation, you either block, approve, or review the content based on your policies and thresholds. You can use machine assistance to augment human moderation of environments where partners, employees, and consumers generate text content. These places include:

Chat rooms

Discussion boards

Chatbots

E-commerce catalogs

Documents

2. Create and subscribe to a Content Moderator resource

Before you can begin to test content moderation or integrate it into your custom applications, you need to create and subscribe to a Content Moderator resource and get the subscription key for accessing the resource.

### Create computer vision solutions with Azure AI Vision
#### Analyze images
1. Provision an Azure AI Vision resource

The Azure AI Vision service is designed to help you extract information from images. It provides functionality that you can use for:

Description and tag generation - determining an appropriate caption for an image, and identifying relevant "tags" that can be used as keywords to indicate its subject.

Object detection - detecting the presence and location of specific objects within the image.

People detection - detecting the presence, location, and features of people in the image.

Image metadata, color, and type analysis - determining the format and size of an image, its dominant color palette, and whether it contains clip art.

Category identification - identifying an appropriate categorization for the image, and if it contains any known landmarks.

Background removal - detecting the background in an image and output the image with the background transparent or a greyscale alpha matte image.

Moderation rating - determine if the image includes any adult or violent content.

Optical character recognition - reading text in the image.

Smart thumbnail generation - identifying the main region of interest in the image to create a smaller "thumbnail" version.

2. Analyze an image:

   To analyze an image, you can use the Analyze Image REST method or the equivalent method in the SDK for your preferred programming language, specifying the visual features you want to include in the analysis (and if you select categories, whether or not to include details of celebrities or landmarks). This method returns a JSON document containing the requested information.

3. Generate a smart-cropped thumbnail and remove background:

   Thumbnails are often used to provide smaller versions of images in applications and websites. For example, a tourism site might display a list of tourist attractions in a city with a small, representative thumbnail image for each attraction; and only display the full image when the user selects the "details" page for an individual attraction.

### Image classification with custom Azure AI Vision models
1. Understand custom model types

Custom Azure AI Vision models have different functionality based on the type. The types of custom models include Image classification, Object detection, and Product recognition.

i. Image classification

ii. Object Dataction

iii. Product Recognition

2. Create a custom project

To create a custom Azure AI Vision model, you first need an Azure AI Services resource (or an Azure AI Vision resource). Once that resource is deployed to your subscription, you need to create a custom project.

3. Label and train a custom model

Once you upload your images to blob storage and created your dataset, the next step is to label your images and connect the resulting COCO file. If you already have a COCO file for your training images, you can skip the labeling step.

Labeling your training images: 
Labeling your training images is done in Azure Machine Learning studio, using the Data Labeling Project. Having complete and accurate labels for your training images greatly improves the performance of your trained model. When you label your images, be sure to accurately assign labels and completely label all instances of each class.

Training your model: 
With all the training images labeled, the next step is training your model. When training a model select the model type, specify the dataset you want to use as training data, and indicate the training budget. The training budget is an upper bound of time for how long the training will run; the actual time used for training is often less than the specified budget.

#### Detect, analyze, and recognize faces
1. Identify options for face detection analysis and identification:
   There are two Azure AI services that you can use to build solutions that detect faces or people in images.

   i. The Azure AI Vision service
   The Azure AI Vision service enables you to detect people in an image, as well as returning a bounding box for its location.

   ii. The Face service
The Face service offers more comprehensive facial analysis capabilities than the Azure AI Vision service, including:

Face detection (with bounding box).

Comprehensive facial feature analysis (including head pose, presence of spectacles, blur, facial landmarks, occlusion and others).

Face comparison and verification.

Facial recognition.

2. Understand considerations for face analysis

While all applications of artificial intelligence require considerations for responsible and ethical use, system that rely on facial data can be particularly problematic.

3. Understand capabilities of the face service

The Face service provides comprehensive facial detection, analysis, and recognition capabilities.

The Face service provides functionality that you can use for:

Face detection - for each detected face, the results include an ID that identifies the face and the bounding box coordinates indicating its location in the image.

Face attribute analysis - you can return a wide range of facial attributes, including:

Head pose (pitch, roll, and yaw orientation in 3D space)

Glasses (NoGlasses, ReadingGlasses, Sunglasses, or Swimming Goggles)

Blur (low, medium, or high)

Exposure (underExposure, goodExposure, or overExposure)

Noise (visual noise in the image)

Occlusion (objects obscuring the face)

Accessories (glasses, headwear, mask)

QualityForRecognition (low, medium, or high)

Facial landmark location - coordinates for key landmarks in relation to facial features (for example, eye corners, pupils, tip of nose, and so on)

Face comparison - you can compare faces across multiple images for similarity (to find individuals with similar facial features) and verification (to determine that a face in one image is the same person as a face in another image)

Facial recognition - you can train a model with a collection of faces belonging to specific individuals, and use the model to identify those people in new images.

Facial liveness - liveness can be used to determine if the input video is a real stream or a fake to prevent bad intentioned individuals from spoofing the recognition system.

4. Compare and match detected faces

When a face is detected by the Face service, a unique ID is assigned to it and retained in the service resource for 24 hours. The ID is a GUID, with no indication of the individual's identity other than their facial features.

5. Implement facial recognition:

   To train a facial recognition model with the Face service:

Create a Person Group that defines the set of individuals you want to identify (for example, employees).
Add a Person to the Person Group for each individual you want to identify.
Add detected faces from multiple images to each person, preferably in various poses. The IDs of these faces will no longer expire after 24 hours (so they're now referred to as persisted faces).
Train the model.

#### Analyze video
1. Understand Azure Video Indexer capabilities

The Azure Video Indexer service is designed to help you extract information from videos. It provides functionality that you can use for:

Facial recognition - detecting the presence of individual people in the image. This requires Limited Access approval.

Optical character recognition - reading text in the video.

Speech transcription - creating a text transcript of spoken dialog in the video.

Topics - identification of key topics discussed in the video.

Sentiment - analysis of how positive or negative segments within the video are.

Labels - label tags that identify key objects or themes throughout the video.

Content moderation - detection of adult or violent themes in the video.

Scene segmentation - a breakdown of the video into its constituent scenes.

2. Extract custom insights

Azure Video Indexer includes predefined models that can recognize well-known celebrities, do OCR, and transcribe spoken phrases into text. You can extend the recognition capabilities of Video Analyzer by creating custom models for:

i. People. Add images of the faces of people you want to recognize in videos, and train a model. Video Indexer will then recognize these people in all of your videos.

ii. Language. If your organization uses specific terminology that may not be in common usage, you can train a custom model to detect and transcribe it.

iii. Brands. You can train a model to recognize specific names as brands, for example to identify products, projects, or companies that are relevant to your business.

3. Use Video Analyzer widgets and APIs

While you can perform all video analysis tasks in the Azure Video Indexer portal, you may want to incorporate the service into custom applications. There are two ways you can accomplish this.

### Develop natural language processing solutions with Azure AI Services.
#### Analyze text with Azure AI Language
1. Provision an Azure AI Language resource

Azure AI Language is designed to help you extract information from text. It provides functionality that you can use for:

Language detection - determining the language in which text is written.

Key phrase extraction - identifying important words and phrases in the text that indicate the main points.

Sentiment analysis - quantifying how positive or negative the text is.

Named entity recognition - detecting references to entities, including people, locations, time periods, organizations, and more.

Entity linking - identifying specific entities by providing reference links to Wikipedia articles.

2. Detect language

The Azure AI Language detection API evaluates text input and, for each document submitted, returns language identifiers with a score indicating the strength of the analysis.

This capability is useful for content stores that collect arbitrary text, where language is unknown. Another scenario could involve a chat bot. If a user starts a session with the chat bot, language detection can be used to determine which language they are using and allow you to configure your bot responses in the appropriate language.

3. Extract key phrases

Key phrase extraction is the process of evaluating the text of a document, or documents, and then identifying the main points around the context of the document(s).

4. Analyze sentiment
5. 
Sentiment analysis is used to evaluate how positive or negative a text document is, which can be useful in various workloads, such as:

Evaluating a movie, book, or product by quantifying sentiment based on reviews.
Prioritizing customer service responses to correspondence received through email or social media messaging.

5. Extract entities

Named Entity Recognition identifies entities that are mentioned in the text. Entities are grouped into categories and subcategories, for example:

Person

Location

DateTime

Organization

Address

Email

URL

6. Extract linked entities

In some cases, the same name might be applicable to more than one entity. For example, does an instance of the word "Venus" refer to the planet or the goddess from mythology?

#### Create question answering solutions with Azure AI Language

1. Understand question answering

Azure AI Language includes a question answering capability, which enables you to define a knowledge base of question and answer pairs that can be queried using natural language input. The knowledge base can be published to a REST endpoint and consumed by client applications, commonly bots.

2. Compare question answering to Azure AI Language understanding

A question answering knowledge base is a form of language model, which raises the question of when to use question answering, and when to use the conversational language understanding capabilities of Azure AI Language.

3. Create a knowledge base

To create a question answering solution, you can use the REST API or SDK to write code that defines, trains, and publishes the knowledge base. However, it's more common to use the Language Studio web interface to define and manage a knowledge base.

To create a knowledge base you:

Sign in to Azure portal.

Search for Azure AI services using the search field at the top of the portal.

Select Create under the Language Service resource.

Create a resource in your Azure subscription:

Enable the question answering feature.

Create or select an Azure AI Search resource to host the knowledge base index.

In Language Studio, select your Azure AI Language resource and create a Custom question answering project.

Add one or more data sources to populate the knowledge base:

URLs for web pages containing FAQs.

Files containing structured text from which questions and answers can be derived.

Predefined chit-chat datasets that include common conversational questions and responses in a specified style.

Edit question and answer pairs in the portal.

4. Implement multi-turn conversation

Although you can often create an effective knowledge base that consists of individual question and answer pairs, sometimes you might need to ask follow-up questions to elicit more information from a user before presenting a definitive answer. This kind of interaction is referred to as a multi-turn conversation.

5. Test and publish a knowledge base

After you have defined a knowledge base, you can train its natural language model, and test it before publishing it for use in an application or bot.

Testing a knowledge base: 
You can test your knowledge base interactively in Language Studio, submitting questions and reviewing the answers that are returned. You can inspect the results to view their confidence scores as well as other potential answers.

Deploying a knowledge base: 
When you are happy with the performance of your knowledge base, you can deploy it to a REST endpoint that client applications can use to submit questions and receive answers. You can deploy it directly from Language Studio.

7. Improve question answering performance:

   Use active learning:
   
Active learning can help you make continuous improvements to get better at answering user questions correctly over time. People often ask questions that are phrased differently, but ultimately have the same meaning. Active learning can help in situations like this because it enables you to consider alternate questions to each question and answer pair. Active learning is enabled by default.

#### Build a conversational language understanding model.
1. Understand prebuilt capabilities of the Azure AI Language service

The Azure AI Language service provides various features for understanding human language. You can use each feature to better communicate with users, better understand incoming communication, or use them together to provide more insight into what the user is saying, intending, and asking about.

2. Understand resources for building a conversational language understanding model

To use the Language Understanding service to develop a NLP solution, you'll need to create a Language resource in Azure. That resource will be used for both authoring your model and processing prediction requests from client applications.

3. Define intents, utterances, and entities

Utterances are the phrases that a user might enter when interacting with an application that uses your language model. An intent represents a task or action the user wants to perform, or more simply the meaning of an utterance. You create a model by defining intents and associating them with one or more utterances.

4. Use patterns to differentiate similar utterances

In some cases, a model might contain multiple intents for which utterances are likely to be similar. You can use the pattern of utterances to disambiguate the intents while minimizing the number of sample utterances.

5. Use pre-built entity components

You can create your own language models by defining all the intents and utterances it requires, but often you can use prebuilt components to detect common entities such as numbers, emails, URLs, or choices.

6. Train, test, publish, and review a conversational language understanding model

   Creating a model is an iterative process with the following activities:

Train a model to learn intents and entities from sample utterances.

Test the model interactively or using a testing dataset with known labels

Deploy a trained model to a public endpoint so client apps can use it

Review predictions and iterate on utterances to train your model

#### Create a custom text classification solution.
1. Understand types of classification projects
Custom text classification assigns labels, which in the Azure AI Language service is a class that the developer defines, to text files. For example, a video game summary might be classified as "Adventure", "Strategy", "Action" or "Sports".

Custom text classification falls into two types of projects:

Single label classification - you can assign only one class to each file. Following the above example, a video game summary could only be classified as "Adventure" or "Strategy".

Multiple label classification - you can assign multiple classes to each file. This type of project would allow you to classify a video game summary as "Adventure" or "Adventure and Strategy".

2. Understand how to build text classification projects

Custom text classification projects are your workspace to build, train, improve, and deploy your classification model. You can work with your project in two ways: through Language Studio and via the REST API. Language Studio is the GUI that will be used in the lab, but the REST API has the same functionality. Regardless of which method you prefer, the steps for developing your model are the same.

#### Custom named entity recognition.
1. Understand custom named entity recognition

Custom NER is an Azure API service that looks at documents, identifies, and extracts user defined entities. These entities could be anything from names and addresses from bank statements to knowledge mining to improve search results.

2. Label your data

Labeling, or tagging, your data correctly is an important part of the process to create a custom entity extraction model. Labels identify examples of specific entities in text used to train the model. Three things to focus on are:

Consistency - Label your data the same way across all files for training. Consistency allows your model to learn without any conflicting inputs.

Precision - Label your entities consistently, without unnecessary extra words. Precision ensures only the correct data is included in your extracted entity.

Completeness - Label your data completely, and don't miss any entities. Completeness helps your model always recognize the entities present.

Train and evaluate your model

Training and evaluating your model is an iterative process of adding data and labels to your training dataset to teach the model more accurately. To know what types of data and labels need to be improved, Language Studio provides scoring in the View model details page on the left hand pane.

#### Translate text with Azure AI Translator service
1. Provision an Azure AI Translator resource

Azure AI Translator provides a multilingual text translation API that you can use for:

Language detection.

One-to-many translation.

Script transliteration (converting text from its native script to an alternative script).

2. Define custom translations

While the default translation model used by Azure AI Translator is effective for general translation, you may need to develop a translation solution for businesses or industries in that have specific vocabularies of terms that require custom translation.

#### Translate text with Azure AI Translator service
1. Provision an Azure resource for speech

Before you can use Azure AI Speech, you need to create an Azure AI Speech resource in your Azure subscription. You can use either a dedicated Azure AI Speech resource or a multi-service Azure AI Services resource.

After you create your resource, you'll need the following information to use it from a client application through one of the supported SDKs:

The location in which the resource is deployed (for example, eastus)

One of the keys assigned to your resource.

2. Use the Azure AI Speech to Text API

The Azure AI Speech service supports speech recognition through two REST APIs:

The Speech to text API, which is the primary way to perform speech recognition.

The Speech to text Short Audio API, which is optimized for short streams of audio.

3. Use the text to speech API

Similarly to its Speech to text APIs, the Azure AI Speech service offers other REST APIs for speech synthesis:

The Text to speech API, which is the primary way to perform speech synthesis.

The Batch synthesis API, which is designed to support batch operations that convert large volumes of text to audio - for example to generate an audio-book from the source text.

4. Configure audio format and voices

When synthesizing speech, you can use a SpeechConfig object to customize the audio that is returned by the Azure AI Speech service.

Audio format:

The Azure AI Speech service supports multiple output formats for the audio stream that is generated by speech synthesis. Depending on your specific needs, you can choose a format based on the required:

Audio file type

Sample-rate

Bit-depth

5. Use Speech Synthesis Markup Language

While the Azure AI Speech SDK enables you to submit plain text to be synthesized into speech (for example, by using the SpeakTextAsync() method), the service also supports an XML-based syntax for describing characteristics of the speech you want to generate. This Speech Synthesis Markup Language (SSML) syntax offers greater control over how the spoken output sounds, enabling you to:

Specify a speaking style, such as "excited" or "cheerful" when using a neural voice.

Insert pauses or silence.

Specify phonemes (phonetic pronunciations), for example to pronounce the text "SQL" as "sequel".

Adjust the prosody of the voice (affecting the pitch, timbre, and speaking rate).

Use common "say-as" rules, for example to specify that a given string should be expressed as a date, time, telephone number, or other form.

Insert recorded speech or audio, for example to include a standard recorded message or simulate background noise.

#### Translate speech with the Azure AI Speech service.
1. Provision an Azure resource for speech translation

The Azure AI Speech service provides robust, machine learning and artificial intelligence-based speech translation services, enabling developers to add end-to-end, real-time, speech translations to their applications or services. You can use either a dedicated Azure AI Speech resource or a multi-service Azure AI Services resource.

2. Translate speech to text

The pattern for speech translation using the Azure AI Speech SDK is similar to speech recognition, with the addition of information about the source and target languages for translation:

3. Synthesize translations

The TranslationRecognizer returns translated transcriptions of spoken input - essentially translating audible speech to text.

You can also synthesize the translation as speech to create speech-to-speech translation solutions. There are two ways you can accomplish this.

i. Event-based synthesis

ii. Manual synthesis

### Implement knowledge mining with Azure AI Search
#### Create an Azure AI Search solution
1. Manage capacity

To create an Azure AI Search solution, you need to create an Azure AI Search resource in your Azure subscription. Depending on the specific solution you intend to build, you may also need Azure resources for data storage and other application services.

2. Understand search components
Completed
100 XP
5 minutes
An AI Search solution consists of multiple components, each playing an important part in the process of extracting, enriching, indexing, and searching data.

i. Data source

ii. Skillset

ii. Indexer

iv. Index

3. Understand the indexing process

The indexing process works by creating a document for each indexed entity. During indexing, an enrichment pipeline iteratively builds the documents that combine metadata from the data source with enriched fields extracted by cognitive skills. You can think of each indexed document as a JSON structure, which initially consists of a document with the index fields you have mapped to fields extracted directly from the source data, like this:

4. Search an index

After you have created and populated an index, you can query it to search for information in the indexed document content. While you could retrieve index entries based on simple field value matching, most search solutions use full text search semantics to query an index.

5. Apply filtering and sorting

It's common in a search solution for users to want to refine query results by filtering and sorting based on field values. Azure AI Search supports both of these capabilities through the search query API.

6. Enhance the index

With a basic index and a client that can submit queries and display results, you can achieve an effective search solution. However, Azure AI Search supports several ways to enhance an index to provide a better user experience. This topic describes some of the ways in which you can extend your search solution.

i. Search-as-you-type

ii. Custom scoring and result boosting

iii. Synonyms

#### Create a custom skill for Azure AI Search
1. Create a custom skill

Your custom skill must implement the expected schema for input and output data that is expected by skills in an Azure AI Search skillset.

2. Add a custom skill to a skillset

To integrate a custom skill into your indexing solution, you must add a skill for it to a skillset using the Custom.WebApiSkill skill type.

The skill definition must:

Specify the URI to your web API endpoint, including parameters and headers if necessary.

Set the context to specify at which point in the document hierarchy the skill should be called

Assign input values, usually from existing document fields

Store output in a new field, optionally specifying a target field name

#### Create a knowledge store with Azure AI Search
1. Define projections

The projections of data to be stored in your knowledge store are based on the document structures generated by the enrichment pipeline in your indexing process. Each skill in your skillset iteratively builds a JSON representation of the enriched data for the documents being indexed, and you can persist some or all of the fields in the document as projections.

2. Define a knowledge store

To define the knowledge store and the projections you want to create in it, you must create a knowledgeStore object in the skillset that specifies the Azure Storage connection string for the storage account where you want to create projections, and the definitions of the projections themselves.

#### Enrich your data with Azure AI Language
1. Explore the available features of Azure AI Language

Here you'll explore the features Azure AI Language offers and then use the demo-like environment to test a preconfigured sentiment model. You'll then see the steps to create, train and deploy a custom model for conversational language understanding.

##### Azure AI Language features

Azure AI Language groups its features into the following areas:

Classify text

Understand questions and conversational language

Extract information

Summarize text

Translate text

2. Enrich a search index in Azure AI Search with custom classes and Azure AI Language

Custom text classification allows you to map a passage of text to different user defined classes. For example, you could train a model on the synopsis on the back cover of books to automatically identify a books genre. You then use that identified genre to enrich your online shop search engine with a genre facet.

#### Implement advanced search features in Azure AI Search
1. Improve the ranking of a document with term boosting

Search works best when the most relevant results are shown first. All search engines try to return the most relevant results to search queries. Azure AI Search implements an enhanced version of Apache Lucene for full text search.

Here, you'll explore how to write more complex Lucene queries. You'll then improve the relevance of results by boosting specific terms in your search query.

Search an index:

Azure AI Search lets you query an index using a REST endpoint or inside the Azure portal with the search explorer tool. If you want a quick recap of the stages of query processing, see the search index unit in Create an Azure AI Search solution.

2. Improve an index with analyzers and tokenized terms

Azure AI Search is configured by default to analyze text and identify tokens that will be helpful in your index. The right tokens ensure that users can find the documents they need quickly. In most cases, the default configuration produces an optimal index. However, when you have unusual or unique fields, you might want to configure exactly how text is analyzed.

3. Enhance an index to include multiple languages

Support for multiple languages can be added to a search index. You can add language support manually by providing all the translated text fields in all the different languages you want to support. You could also choose to use Azure AI Services to provide translated text through an enrichment pipeline.

4. Improve search experience by ordering results by distance from a given reference point

Often, users want to search for items associated with a geographical location. For example, they might want to find the nearest coffee shop to their location. To help you compare locations on the Earth's surface, AI Search includes geo-spatial functions that you can call in queries.

#### Build an Azure Machine Learning custom skill for Azure AI Search
1. Understand how to use a custom Azure Machine Learning skillset

Using a machine learning custom skill works the same as adding any other custom skill to a search index.

Here, you'll see how using the AmlSkill custom skill is different and explore the considerations of how to effectively use it.

2. Enrich a search index using an Azure Machine Learning model

You create your Azure Machine Learning model using developer tools like the Python SDK, REST APIs, or Azure CLI. Another option is to take advantage of the Azure AI Machine Learning studio, a graphical user interface that lets you create, train, and deploy models without writing any code.

#### Search data outside the Azure platform in Azure AI Search using Azure Data Factory
1. Index data from external data sources using Azure Data Factory

Adding external data that doesn't reside in Azure is a common need in an organization's search solution. Azure AI Search is flexible as it allows many ways to create and push data into indexes.

2. Index any data using the Azure AI Search push API

The REST API is the most flexible way to push data into an Azure AI Search index. You can use any programming language or interactively with any app that can post JSON requests to an endpoint.

#### Maintain an Azure AI Search solution
1. Manage security of an Azure AI Search solution

Organizations need to be able to trust the security of their search solutions. Azure AI Search gives you control over how to secure the data you search.

2. Optimize performance of an Azure AI Search solution

Your search solutions performance can be affected by the size and complexity of your indexes. You also need to know how to write efficient queries to search it and choose the right service tier.

3. Manage costs of an Azure AI Search solution

The costs of running an Azure AI Search solution vary depending on the capacity and features you use.

4. Improve reliability of an Azure AI Search solution

Now you've a well-managed, secured, and cost-effective search solution. The next step is to make sure your service is highly available and protected from disasters.

5. Monitor an Azure AI Search solution

Azure Monitor can give you insights into how well your search service is being used and performing. You can also receive alerts to proactively notify you of issues.

6. Debug search issues using the Azure portal

When you first create your search service, you have to make some assumptions about the data you are indexing. You make choices about the index and how to ingest that data. However, until you run your created indexer you can't be certain that you made all the correct choices.

#### Perform search re-ranking with semantic ranking in Azure AI Search
1. What is semantic ranking?

Semantic ranking is a capability within Azure AI Search that aims to improve the ranking of search results. Semantic ranking improves the ranking of search results by using language understanding to more accurately match the context of the original query.

2. Set up semantic ranking

You can enable semantic ranking at the service level and once it is enabled, semantic ranking is available for all indexes. Semantic ranking cannot be enabled or disabled on a per-index basis.

#### Perform vector search and retrieval in Azure AI Search
1. What is vector search?

Vector search is a new capability available in AI Search used to index, store and retrieve vector embedding from a search index. You can use it to power applications implementing the Retrieval Augmented Generation (RAG) architecture, similarity and multi-modal searches or recommendation engines.

2. Prepare your search

You need to encode your Azure AI Search query by sending it to an embedded model. The response is then passed to a search engine to complete a search over the vector fields.

3. nderstand embedding

An embedding is type of data representation that is used by machine learning models. An embedding represents the semantic meaning of a piece of text. You can visualize an embedding as an array of numbers, and the numerical distance between two embeddings represents their semantic similarity. For example, if two texts are similar, then their representations should also be similar.

### Develop Generative AI solutions with Azure OpenAI Service
#### Get started with Azure OpenAI Service
1. Create an Azure OpenAI Service resource in the Azure portal
When you create an Azure OpenAI Service resource, you need to provide a subscription name, resource group name, region, unique instance name, and select a pricing tier.

2. Use Azure OpenAI Studio

Azure OpenAI Studio provides access to model management, deployment, experimentation, customization, and learning resources.

You can access the Azure OpenAI Studio through the Azure portal after creating a resource, or at https://oai.azure.com by logging in with your Azure OpenAI resource instance. During the sign-in workflow, select the appropriate directory, Azure subscription, and Azure OpenAI resource.

3. Explore types of generative AI models

To begin building with Azure OpenAI, you need to choose a base model and deploy it. Microsoft provides base models and the option to create customized base models. This module covers the currently available base models.

Azure OpenAI includes several types of model:

i. GPT 4 model
ii. GPT 3.5 model 
iii. Embeddings models
iv Dall-E model

4. Deploy generative AI models

You first need to deploy a model to make API calls to receive completions to prompts. When you create a new deployment, you need to indicate which base model to deploy. You can deploy any number of deployments in one or multiple Azure OpenAI resources as long as their TPM adds up to less than 240K total in that region. There are several ways you can deploy your base model.

5. Test models in Azure OpenAI Studio's playgrounds

Playgrounds are useful interfaces in Azure OpenAI Studio that you can use to experiment with your deployed models without needing to develop your own client application. Azure OpenAI Studio offers multiple playgrounds with different parameter tuning options.


#### Build natural language solutions with Azure OpenAI Service
1. Integrate Azure OpenAI into your app

Azure OpenAI offers both C# and Python SDKs and a REST API that developers can use to add AI functionality to their applications. Generative AI capabilities in Azure OpenAI are provided through models. The models available in the Azure OpenAI service belong to different families, each with their own focus. To use one of these models, you need to deploy through the Azure OpenAI Service.

#### Apply prompt engineering with Azure OpenAI Service
1. Understand prompt engineering

The quality of the input prompts we send to an AI model, like those available in Azure OpenAI, directly influences the quality of what we get back. By carefully constructing the prompts we send to the model, the model can provide better and more interesting responses.

2. Write more effective prompts

Azure OpenAI models are capable of generating responses to natural language queries with remarkable accuracy. However, the quality of the responses depends largely on how well the prompt is written. Developers can optimize the performance of Azure OpenAI models by using different techniques in their prompts, resulting in more accurate and relevant responses.

Provide clear instructions:
Asking the Azure OpenAI model clearly for what you want is one way to get desired results. By being as descriptive as possible, the model can generate a response that most closely matches what you're looking for.

#### Generate code with Azure OpenAI Service
1. Construct code from natural language

One of the capabilities of Azure OpenAI models is to generate code from natural language prompts. Tasks can range from a simple one line command to a full application. The AI models can also edit and update provided code or previous responses to complete the requested task.

AI models for code generation:

In previous generations of gpt models, some were trained specifically for use with code (often called codex models). As new generations of models evolve, the base models drastically improve their performance and understanding of both language and code, which results in not needing specific code models. This improvement results in just a single model for more recent generations (such as gpt-35-turbo and gpt-4) that can be used for both natural language and code.

2. Fix bugs and improve your code

Developers sometimes can write code that mostly works, but could be improved by fixing bugs, syntax, performance, or modularity. Azure OpenAI models can help identify ways to improve and provide suggestions on how to write better code.

Fix bugs in your code:

Azure OpenAI models can help fix bugs in code by analyzing the code and suggesting changes that can potentially fix the issue. This can help developers identify and resolve bugs faster and more efficiently.

#### Generate images with Azure OpenAI Service
1. What is DALL-E?

DALL-E is a neural network based model that can generate graphical data from natural language input. Put more simply, you can provide DALL-E with a description and it can generate an appropriate image.

#### Implement Retrieval Augmented Generation (RAG) with Azure OpenAI Service
1. Understand Retrieval Augmented Generation (RAG) with Azure OpenAI Service

RAG with Azure OpenAI allows developers to use supported AI chat models that can reference specific sources of information to ground the response. Adding this information allows the model to reference both the specific data provided and its pretrained knowledge to provide more effective responses.

Azure OpenAI enables RAG by connecting pretrained models to your own data sources. Azure OpenAI on your data utilizes the search ability of Azure AI Search to add the relevant data chunks to the prompt. Once your data is in a AI Search index, Azure OpenAI on your data goes through the following steps:

Receive user prompt.

Determine relevant content and intent of the prompt.

Query the search index with that content and intent.

Insert search result chunk into the Azure OpenAI prompt, along with system message and user prompt.

Send entire prompt to Azure OpenAI.

response and data reference (if any) to the user.

By default, Azure OpenAI on your data encourages, but doesn't require, the model to respond only using your data. This setting can be unselected when connecting your data, which may result in the model choosing to use its pretrained knowledge over your data.

2. Add your own data source

Adding your data is done through the Azure OpenAI Studio, in the Chat playground. The data source you add is then used to augment the prompt sent to the model. When adding your data, you can choose to upload your data files, use data in a blob storage account, or connect to an existing AI Search index.

If you're uploading or using files already in a storage account, Azure OpenAI on your data supports .md, .txt, .html, .pdf, and Microsoft Word or PowerPoint files. If any of these files contain graphics or images, the response quality depends on how well text can be extracted from the visual content.

When uploading data or connecting to files in a storage account, it's recommended to use the Azure OpenAI Studio to create the search resource and index. Adding data this way allows the appropriate chunking to happen when inserting into the index, yielding better responses. If you're using large text files or forms, you should use the available data preparation script to improve the AI model's accuracy.

Enabling semantic search for your AI Search service can improve the result of searching your data index and you're likely to receive higher quality responses and citations. However, enabling semantic search may increase the cost of the search service.

3. Chat with your model using your own data

RAG with Azure OpenAI on your own data can be used in Azure OpenAI Studio with the Chat playground, or by using the API.

Token considerations and recommended settings
Since RAG with Azure OpenAI on your data includes search results on your index in the prompt, it's important to understand how that impacts your token allotment. Each call to the model includes tokens for the system message, the user prompt, conversation history, retrieved search documents, internal prompts, and the model's response.

The system message, for example, is a useful reference for instructions for the model and is included with every call. While there's no token limit for the system message, when using your own data the system message gets truncated if it exceeds 200 tokens. The response from the model is also limited when using your own data is 1500 tokens.

Due to these token limitations, it's recommended that you limit both the question length and the conversation history length in your call. Prompt engineering techniques such as breaking down the task and chain of thought prompting can help the model respond more effectively.

### Fundamentals of Responsible Generative AI
1. Plan a responsible generative AI solution

The Microsoft guidance for responsible generative AI is designed to be practical and actionable. It defines a four stage process to develop and implement a plan for responsible AI when using generative models. The four stages in the process are:

Identify potential harms that are relevant to your planned solution.

Measure the presence of these harms in the outputs generated by your solution.

Mitigate the harms at multiple layers in your solution to minimize their presence and impact, and ensure transparent communication about 
potential risks to users.

Operate the solution responsibly by defining and following a deployment and operational readiness plan.

2. Identify potential harms

The first stage in a responsible generative AI process is to identify the potential harms that could affect your planned solution. There are four steps in this stage, as shown here:

Identify potential harms

Prioritize identified harms

Test and verify the prioritized harms

Document and share the verified harms

3. Measure potential harms

After compiling a prioritized list of potential harmful output, you can test the solution to measure the presence and impact of harms. Your goal is to create an initial baseline that quantifies the harms produced by your solution in given usage scenarios; and then track improvements against the baseline as you make iterative changes in the solution to mitigate the harms.

Manual and automatic testing:

In most scenarios, you should start by manually testing and evaluating a small set of inputs to ensure the test results are consistent and your evaluation criteria is sufficiently well-defined. Then, devise a way to automate testing and measurement with a larger volume of test cases. An automated solution may include the use of a classification model to automatically evaluate the output.

4. Operate a responsible generative AI solution

When you have identified potential harms, developed a way to measure their presence, and implemented mitigations for them in your solution, you can get ready to release your solution. Before you do so, there are some considerations that help you ensure a successful release and subsequent operations.
