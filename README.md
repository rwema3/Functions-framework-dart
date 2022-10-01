## Functions Framework for Dart
>This is a community-supported project, meaning there is no official level of support. The code is not covered by any SLA or deprecation policy.

An open source FaaS (Function as a Service) framework for writing portable Dart functions, brought to you by Open Source Developer Rwema

The Functions Framework lets you write lightweight functions that run in many different environments, including:

Your local development machine
Google Cloud Run - see cloud run quickstart
Google App Engine
Knative-based environments
Google Cloud Functions does not currently provide an officially supported Dart language runtime, but we're working to make running on Google Cloud Run as seamless and symmetric an experience as possible for your Dart Functions Framework projects.

The framework allows you to go from:

examples/hello/lib/functions.dart

import 'package:functions_framework/functions_framework.dart';
import 'package:shelf/shelf.dart';

@CloudFunction()
Response function(Request request) => Response.ok('Hello, World!');
