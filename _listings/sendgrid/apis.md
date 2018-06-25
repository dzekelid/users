---
name: SendGrid
x-slug: sendgrid
description: Delivering your transactional and marketing emails through the worlds
  largest cloud-based email delivery platform. Send with confidence.
image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/142-sendgrid.jpg
x-kinRank: "9"
x-alexaRank: "10000"
tags: Users
created: "2018-06-25"
modified: "2018-06-25"
url: https://raw.githubusercontent.com/streamdata-gallery-topics/users/master/_listings/sendgrid/apis.md
specificationVersion: "0.14"
apis:
- name: SendGrid Get Subusers
  x-api-slug: sendgrid
  description: |-
    This endpoint allows you to retrieve a list of all of your subusers. You can choose to retrieve specific subusers as well as limit the results that come back from the API.

    For more information about Subusers:

    * [User Guide > Subusers](https://sendgrid.com/docs/User_Guide/Settings/Subusers/index.html)
    * [Classroom > How do I add more subusers to my account?](https://sendgrid.com/docs/Classroom/Basics/Account/how_do_i_add_more_subusers_to_my_account.html)
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/142-sendgrid.jpg
  humanURL: http://sendgrid.com
  baseURL: https://api.sendgrid.com//v3//subusers
  tags: Email,Subusers
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/users/master/_listings/sendgrid/subusers-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/users/master/_listings/sendgrid/subusers-get-openapi.md
- name: SendGrid Add Subusers
  x-api-slug: sendgrid
  description: |-
    This endpoint allows you to retrieve a list of all of your subusers. You can choose to retrieve specific subusers as well as limit the results that come back from the API.

    For more information about Subusers:

    * [User Guide > Subusers](https://sendgrid.com/docs/User_Guide/Settings/Subusers/index.html)
    * [Classroom > How do I add more subusers to my account?](https://sendgrid.com/docs/Classroom/Basics/Account/how_do_i_add_more_subusers_to_my_account.html)
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/142-sendgrid.jpg
  humanURL: http://sendgrid.com
  baseURL: https://api.sendgrid.com//v3//subusers
  tags: Email,Subusers
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/users/master/_listings/sendgrid/subusers-post-openapi.md
- name: SendGrid Get Subusers Reputations
  x-api-slug: sendgrid
  description: |-
    Subuser sender reputations give a good idea how well a sender is doing with regards to how recipients and recipient servers react to the mail that is being received. When a bounce, spam report, or other negative action happens on a sent email, it will effect your sender rating.

    This endpoint allows you to request the reputations for your subusers.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/142-sendgrid.jpg
  humanURL: http://sendgrid.com
  baseURL: https://api.sendgrid.com//v3//subusers/reputations
  tags: Email,Subusers, Reputations
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/users/master/_listings/sendgrid/subusersreputations-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/users/master/_listings/sendgrid/subusersreputations-get-openapi.md
- name: SendGrid Get Subusers Stats
  x-api-slug: sendgrid
  description: |-
    **This endpoint allows you to retrieve the email statistics for the given subusers.**

    You may retrieve statistics for up to 10 different subusers by including an additional _subusers_ parameter for each additional subuser.

    While you can always view the statistics for all email activity on your account, subuser statistics enable you to view specific segments of your stats. Emails sent, bounces, and spam reports are always tracked for subusers. Unsubscribes, clicks, and opens are tracked if you have enabled the required settings.

    For more information, see our [User Guide](https://sendgrid.com/docs/User_Guide/Statistics/subuser.html).
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/142-sendgrid.jpg
  humanURL: http://sendgrid.com
  baseURL: https://api.sendgrid.com//v3//subusers/stats
  tags: Email,Subusers, Stats
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/users/master/_listings/sendgrid/subusersstats-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/users/master/_listings/sendgrid/subusersstats-get-openapi.md
- name: SendGrid Get Subusers Stats Monthly
  x-api-slug: sendgrid
  description: |-
    **This endpoint allows you to retrieve the monthly email statistics for all subusers over the given date range.**

    While you can always view the statistics for all email activity on your account, subuser statistics enable you to view specific segments of your stats for your subusers. Emails sent, bounces, and spam reports are always tracked for subusers. Unsubscribes, clicks, and opens are tracked if you have enabled the required settings.

    When using the `sort_by_metric` to sort your stats by a specific metric, you can not sort by the following metrics:
    `bounce_drops`, `deferred`, `invalid_emails`, `processed`, `spam_report_drops`, `spam_reports`, or `unsubscribe_drops`.

    For more information, see our [User Guide](https://sendgrid.com/docs/User_Guide/Statistics/subuser.html).
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/142-sendgrid.jpg
  humanURL: http://sendgrid.com
  baseURL: https://api.sendgrid.com//v3//subusers/stats/monthly
  tags: Email,Subusers, Stats, Monthly
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/users/master/_listings/sendgrid/subusersstatsmonthly-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/users/master/_listings/sendgrid/subusersstatsmonthly-get-openapi.md
- name: SendGrid Get Subusers Stats Sums
  x-api-slug: sendgrid
  description: |-
    **This endpoint allows you to retrieve the total sums of each email statistic metric for all subusers over the given date range.**


    While you can always view the statistics for all email activity on your account, subuser statistics enable you to view specific segments of your stats. Emails sent, bounces, and spam reports are always tracked for subusers. Unsubscribes, clicks, and opens are tracked if you have enabled the required settings.

    For more information, see our [User Guide](https://sendgrid.com/docs/User_Guide/Statistics/subuser.html).
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/142-sendgrid.jpg
  humanURL: http://sendgrid.com
  baseURL: https://api.sendgrid.com//v3//subusers/stats/sums
  tags: Email,Subusers, Stats, Sums
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/users/master/_listings/sendgrid/subusersstatssums-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/users/master/_listings/sendgrid/subusersstatssums-get-openapi.md
- name: SendGrid Delete Subusers Subuser Name
  x-api-slug: sendgrid
  description: |-
    This endpoint allows you to delete a subuser. This is a permanent action, once deleted a subuser cannot be retrieved.

    For more information about Subusers:

    * [User Guide > Subusers](https://sendgrid.com/docs/User_Guide/Settings/Subusers/index.html)
    * [Classroom > How do I add more subusers to my account?](https://sendgrid.com/docs/Classroom/Basics/Account/how_do_i_add_more_subusers_to_my_account.html)
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/142-sendgrid.jpg
  humanURL: http://sendgrid.com
  baseURL: https://api.sendgrid.com//v3//subusers/{subuser_name}
  tags: Email,Subusers, Subuser, Name
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/users/master/_listings/sendgrid/subuserssubuser-name-delete-openapi.md
- name: SendGrid Patch Subusers Subuser Name
  x-api-slug: sendgrid
  description: |-
    This endpoint allows you to enable or disable a subuser.

    For more information about Subusers:

    * [User Guide > Subusers](https://sendgrid.com/docs/User_Guide/Settings/Subusers/index.html)
    * [Classroom > How do I add more subusers to my account?](https://sendgrid.com/docs/Classroom/Basics/Account/how_do_i_add_more_subusers_to_my_account.html)
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/142-sendgrid.jpg
  humanURL: http://sendgrid.com
  baseURL: https://api.sendgrid.com//v3//subusers/{subuser_name}
  tags: Email,Subusers, Subuser, Name
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/users/master/_listings/sendgrid/subuserssubuser-name-patch-openapi.md
- name: SendGrid Put Subusers Subuser Name Ips
  x-api-slug: sendgrid
  description: "Each subuser should be assigned to an IP address, from which all of
    this subuser's mail will be sent. Often, this is the same IP as the parent account,
    but each subuser can have their own, or multiple, IP addresses as well. \n\nMore
    information:\n\n* [How to request more IPs](https://sendgrid.com/docs/Classroom/Basics/Account/adding_an_additional_dedicated_ip_to_your_account.html)\n*
    [IPs can be whitelabeled](https://sendgrid.com/docs/User_Guide/Settings/Whitelabel/ips.html)"
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/142-sendgrid.jpg
  humanURL: http://sendgrid.com
  baseURL: https://api.sendgrid.com//v3//subusers/{subuser_name}/ips
  tags: Email,Subusers, Subuser, Name, Ips
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/users/master/_listings/sendgrid/subuserssubuser-nameips-put-openapi.md
- name: SendGrid Delete Subusers Subuser Name Monitor
  x-api-slug: sendgrid
  description: Subuser monitor settings allow you to receive a sample of an outgoing
    message by a specific customer at a specific frequency of emails.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/142-sendgrid.jpg
  humanURL: http://sendgrid.com
  baseURL: https://api.sendgrid.com//v3//subusers/{subuser_name}/monitor
  tags: Email,Subusers, Subuser, Name, Monitor
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/users/master/_listings/sendgrid/subuserssubuser-namemonitor-delete-openapi.md
- name: SendGrid Get Subusers Subuser Name Monitor
  x-api-slug: sendgrid
  description: Subuser monitor settings allow you to receive a sample of an outgoing
    message by a specific customer at a specific frequency of emails.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/142-sendgrid.jpg
  humanURL: http://sendgrid.com
  baseURL: https://api.sendgrid.com//v3//subusers/{subuser_name}/monitor
  tags: Email,Subusers, Subuser, Name, Monitor
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/users/master/_listings/sendgrid/subuserssubuser-namemonitor-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/users/master/_listings/sendgrid/subuserssubuser-namemonitor-get-openapi.md
- name: SendGrid Add Subusers Subuser Name Monitor
  x-api-slug: sendgrid
  description: Subuser monitor settings allow you to receive a sample of an outgoing
    message by a specific customer at a specific frequency of emails.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/142-sendgrid.jpg
  humanURL: http://sendgrid.com
  baseURL: https://api.sendgrid.com//v3//subusers/{subuser_name}/monitor
  tags: Email,Subusers, Subuser, Name, Monitor
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/users/master/_listings/sendgrid/subuserssubuser-namemonitor-post-openapi.md
- name: SendGrid Put Subusers Subuser Name Monitor
  x-api-slug: sendgrid
  description: Subuser monitor settings allow you to receive a sample of an outgoing
    message by a specific customer at a specific frequency of emails.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/142-sendgrid.jpg
  humanURL: http://sendgrid.com
  baseURL: https://api.sendgrid.com//v3//subusers/{subuser_name}/monitor
  tags: Email,Subusers, Subuser, Name, Monitor
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/users/master/_listings/sendgrid/subuserssubuser-namemonitor-put-openapi.md
- name: SendGrid Get Subusers Subuser Name Stats Monthly
  x-api-slug: sendgrid
  description: |-
    **This endpoint allows you to retrive the monthly email statistics for a specific subuser.**

    While you can always view the statistics for all email activity on your account, subuser statistics enable you to view specific segments of your stats for your subusers. Emails sent, bounces, and spam reports are always tracked for subusers. Unsubscribes, clicks, and opens are tracked if you have enabled the required settings.

    When using the `sort_by_metric` to sort your stats by a specific metric, you can not sort by the following metrics:
    `bounce_drops`, `deferred`, `invalid_emails`, `processed`, `spam_report_drops`, `spam_reports`, or `unsubscribe_drops`.

    For more information, see our [User Guide](https://sendgrid.com/docs/User_Guide/Statistics/subuser.html).
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/142-sendgrid.jpg
  humanURL: http://sendgrid.com
  baseURL: https://api.sendgrid.com//v3//subusers/{subuser_name}/stats/monthly
  tags: Email,Subusers, Subuser, Name, Stats, Monthly
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/users/master/_listings/sendgrid/subuserssubuser-namestatsmonthly-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/users/master/_listings/sendgrid/subuserssubuser-namestatsmonthly-get-openapi.md
- name: SendGrid
  x-api-slug: sendgrid
  description: SendGrids cloud-based email infrastructure relieves businesses of the
    cost and complexity of maintaining custom email systems. SendGrid provides reliable
    delivery, scalability and real-time analytics along with flexible APIs that make
    custom integration a breeze.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/142-sendgrid.jpg
  humanURL: http://sendgrid.com
  baseURL: https://api.sendgrid.com//v3
  tags: Users
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/users/master/_listings/sendgrid/openapi.md
x-common:
- type: x--net-library
  url: https://sendgrid.com/docs/Code_Examples/csharp.html
- type: x-base
  url: https://api.sendgrid.com
- type: x-blog
  url: http://blog.sendgrid.com/
- type: x-blog-rss
  url: http://feeds.feedburner.com/sendgrid/CDXr
- type: x-contact-form
  url: https://sendgrid.com/contact
- type: x-crunchbase
  url: http://www.crunchbase.com/company/sendgrid
- type: x-crunchbase
  url: https://crunchbase.com/organization/sendgrid
- type: x-developer
  url: https://sendgrid.com/developers
- type: x-documentation
  url: https://sendgrid.com/docs/index.html
- type: x-email
  url: privacy@sendgrid.com
- type: x-email
  url: legal@sendgrid.com
- type: x-email
  url: dpo@sendgrid.com
- type: x-forum
  url: http://support.sendgrid.com/forums
- type: x-github
  url: https://github.com/sendgrid
- type: x-go-library
  url: https://sendgrid.com/docs/Code_Examples/go.html
- type: x-ios-library
  url: https://sendgrid.com/docs/Code_Examples/ios.html
- type: x-java-library
  url: https://sendgrid.com/docs/Code_Examples/java.html
- type: x-labs
  url: http://labs.sendgrid.com/
- type: x-linkedin
  url: https://www.linkedin.com/company/sendgrid
- type: x-node-js-library
  url: https://sendgrid.com/docs/Code_Examples/nodejs.html
- type: x-partners
  url: https://sendgrid.com/partners
- type: x-perl-library
  url: https://sendgrid.com/docs/Code_Examples/perl.html
- type: x-php-library
  url: https://sendgrid.com/docs/Code_Examples/php.html
- type: x-pricing
  url: https://sendgrid.com/transactional-email/pricing
- type: x-privacy
  url: https://sendgrid.com/privacy
- type: x-python-library
  url: https://sendgrid.com/docs/Code_Examples/python.html
- type: x-ruby-library
  url: https://sendgrid.com/docs/Code_Examples/ruby.html
- type: x-security
  url: https://sendgrid.com/security
- type: x-selfservice-registration
  url: https://sendgrid.com/user/signup
- type: x-terms-of-service
  url: https://sendgrid.com/tos
- type: x-twitter
  url: https://twitter.com/SendGrid
- type: x-website
  url: http://sendgrid.com
- type: x-website
  url: https://sendgrid.com/
include: []
maintainers:
- FN: Kin Lane
  x-twitter: apievangelist
  email: info@apievangelist.com
---