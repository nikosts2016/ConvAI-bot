# ConvAI bot#

Skill-based Conversational Agent


# Abstract

The chatbot developed for the diploma thesis. ConvAI bot is
capable of conversing with humans about given text (e.g. a paragraph from
Wikipedia article). The conversation is enabled by a set of skills, including
chit-chat, topics detection, text summarization, question answering and question
generation. The system has been trained in a supervised fashion to select an
appropriate skill for generating a response. Furthermore, it has been developed an
overall dialog quality scorer and next utterance scorer to correct agent's
policy. This bot is implemented with open source software and open data; it is
self-hosted, and employs a supervised dialog manager with a linear hierarchy.
The latter allows a researcher to focus on skill implementation rather than
finite state machine development.


## Prerequisites

- Docker version 17.05.0-ce+
- docker-compose version 1.13.0+
- Min. 4 Gb RAM + Swap (4 Gb), recommended 8 Gb RAM
- 2 Gb hard drive space
- Tested on Ubuntu 16.04
