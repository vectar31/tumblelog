# tumblelog

URL = "https://docs.mongodb.org/ecosystem/tutorial/write-a-tumblelog-application-with-flask-mongoengine/"

Introduction

This tutorial describes the process for creating a basic tumblelog application using the popular Flask Python web-framework in conjunction with the MongoDB database.

The tumblelog will consist of two parts:

A public site that lets people view posts and comment on them.
An admin site that lets you add and change posts.
This tutorial assumes that you are already familiar with Flask and have a basic familiarity with MongoDB and have installed MongoDB. This tutorial uses MongoEngine as the Object Document Mapper (ODM,) this component may simplify the interaction between Flask and MongoDB.

WHERE TO GET HELP
If you’re having trouble going through this tutorial, please post a message to mongodb-user or join the IRC chat in #mongodb on irc.freenode.net to chat with other MongoDB users who might be able to help.
Installation

Begin by installing packages required by later steps in this tutorial.

Prerequisite
This tutorial uses pip to install packages and virtualenv to isolate Python environments. While these tools and this configuration are not required as such, they ensure a standard environment and are strongly recommended. Issue the following command at the system prompt:

pip install virtualenv
virtualenv myproject
Respectively, these commands: install the virtualenv program (using pip) and create an isolated Python environment for this project (named myproject.)

To activate myproject environment at the system prompt, use the following command:

source myproject/bin/activate
Install Packages
Flask is a “microframework,” because it provides a small core of functionality and is highly extensible. For the “tumblelog” project, this tutorial includes task and the following extension:

WTForms provides easy form handling.
Flask-MongoEngine provides integration between MongoEngine, Flask, and WTForms.
Flask-Script for an easy-to-use development server
Install with the following commands:

pip install flask
pip install flask-script
pip install WTForms
pip install mongoengine
pip install flask_mongoengine

Continue with the tutorial to begin building the “tumblelog” application.