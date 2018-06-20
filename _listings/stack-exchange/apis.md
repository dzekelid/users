---
name: Stack Exchange
x-slug: stack-exchange
description: After someone asks a question, members of the community propose answers.
  Others vote on those answers. Very quickly, the answers with the most votes rise
  to the top. You don???t have to read through a lot of discussion to find the best
  answer.    Like to...
image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/253-stack-exchange.jpg
x-kinRank: "8"
x-alexaRank: "126"
tags: Users
created: "2018-06-20"
modified: "2018-06-20"
url: https://raw.githubusercontent.com/streamdata-gallery-topics/users/master/_listings/stack-exchange/apis.md
specificationVersion: "0.14"
apis:
- name: Stack Exchange Get Users
  x-api-slug: stack-exchange
  description: "Returns all users on a site.\n \nThis method returns a list of users.\n
    \nThe sorts accepted by this method operate on the follow fields of the user object:\n
    - reputation - reputation\n - creation - creation_date\n - name - display_name\n
    - modified - last_modified_date\n  reputation is the default sort.\n \n It is
    possible to create moderately complex queries using sort, min, max, fromdate,
    and todate.\n \nThe inname parameter lets consumers filter the results down to
    just those users with a certain substring in their display name. For example,
    inname=kevin will return all users with both users named simply \"Kevin\" or those
    with Kevin as one of (or part of) their names; such as \"Kevin Montrose\"."
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/253-stack-exchange.jpg
  humanURL: http://stackexchange.com
  baseURL: https://api.stackexchange.com//2.2//users
  tags: Users
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/users/master/_listings/stack-exchange/users-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/users/master/_listings/stack-exchange/users-get-openapi.md
- name: Stack Exchange Get User Moderators
  x-api-slug: stack-exchange
  description: "Gets those users on a site who can exercise moderation powers.\n \nNote,
    employees of Stack Exchange Inc. will be returned if they have been granted moderation
    powers on a site even if they have never been appointed or elected explicitly.
    This method checks abilities, not the manner in which they were obtained.\n \nThe
    sorts accepted by this method operate on the follow fields of the user object:\n
    - reputation - reputation\n - creation - creation_date\n - name - display_name\n
    - modified - last_modified_date\n  reputation is the default sort.\n \n It is
    possible to create moderately complex queries using sort, min, max, fromdate,
    and todate.\n \nThis method returns a list of users."
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/253-stack-exchange.jpg
  humanURL: http://stackexchange.com
  baseURL: https://api.stackexchange.com//2.2//users/moderators
  tags: Users,Moderators
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/users/master/_listings/stack-exchange/usersmoderators-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/users/master/_listings/stack-exchange/usersmoderators-get-openapi.md
- name: Stack Exchange Get Users Moderators Elected
  x-api-slug: stack-exchange
  description: "Returns those users on a site who both have moderator powers, and
    were actually elected.\n \nThis method excludes Stack Exchange Inc. employees,
    unless they were actually elected moderators on a site (which can only have happened
    prior to their employment).\n \nThe sorts accepted by this method operate on the
    follow fields of the user object:\n - reputation - reputation\n - creation - creation_date\n
    - name - display_name\n - modified - last_modified_date\n  reputation is the default
    sort.\n \n It is possible to create moderately complex queries using sort, min,
    max, fromdate, and todate.\n \nThis method returns a list of users."
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/253-stack-exchange.jpg
  humanURL: http://stackexchange.com
  baseURL: https://api.stackexchange.com//2.2//users/moderators/elected
  tags: Users,Moderators
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/users/master/_listings/stack-exchange/usersmoderatorselected-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/users/master/_listings/stack-exchange/usersmoderatorselected-get-openapi.md
- name: Stack Exchange Get User
  x-api-slug: stack-exchange
  description: "Gets the users identified in ids in {ids}.\n \nTypically this method
    will be called to fetch user profiles when you have obtained user ids from some
    other source, such as /questions.\n \n{ids} can contain up to 100 semicolon delimited
    ids, to find ids programatically look for user_id on user or shallow_user objects.\n
    \nThe sorts accepted by this method operate on the follow fields of the user object:\n
    - reputation - reputation\n - creation - creation_date\n - name - display_name\n
    - modified - last_modified_date\n  reputation is the default sort.\n \n It is
    possible to create moderately complex queries using sort, min, max, fromdate,
    and todate.\n \nThis method returns a list of users."
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/253-stack-exchange.jpg
  humanURL: http://stackexchange.com
  baseURL: https://api.stackexchange.com//2.2//users/{ids}
  tags: Users
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/users/master/_listings/stack-exchange/usersids-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/users/master/_listings/stack-exchange/usersids-get-openapi.md
- name: Stack Exchange Get User Answers
  x-api-slug: stack-exchange
  description: "Returns the answers the users in {ids} have posted.\n \n{ids} can
    contain up to 100 semicolon delimited ids, to find ids programatically look for
    user_id on user or shallow_user objects.\n \nThe sorts accepted by this method
    operate on the follow fields of the answer object:\n - activity - last_activity_date\n
    - creation - creation_date\n - votes - score\n  activity is the default sort.\n
    \n It is possible to create moderately complex queries using sort, min, max, fromdate,
    and todate.\n \nThis method returns a list of answers."
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/253-stack-exchange.jpg
  humanURL: http://stackexchange.com
  baseURL: https://api.stackexchange.com//2.2//users/{ids}/answers
  tags: Users,Answers
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/users/master/_listings/stack-exchange/usersidsanswers-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/users/master/_listings/stack-exchange/usersidsanswers-get-openapi.md
- name: Stack Exchange Get User Associated
  x-api-slug: stack-exchange
  description: "Returns all of a user's associated accounts, given their account_ids
    in {ids}.\n \n{ids} can contain up to 100 semicolon delimited ids, to find ids
    programatically look for account_id on user objects.\n \nThis method returns a
    list of network_users."
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/253-stack-exchange.jpg
  humanURL: http://stackexchange.com
  baseURL: https://api.stackexchange.com//2.2//users/{ids}/associated
  tags: Users,Associated
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/users/master/_listings/stack-exchange/usersidsassociated-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/users/master/_listings/stack-exchange/usersidsassociated-get-openapi.md
- name: Stack Exchange Get User Badges
  x-api-slug: stack-exchange
  description: "Get the badges the users in {ids} have earned.\n \nBadge sorts are
    a tad complicated. For the purposes of sorting (and min/max) tag_based is considered
    to be greater than named.\n \nThis means that you can get a list of all tag based
    badges a user has by passing min=tag_based, and conversely all the named badges
    by passing max=named, with sort=type.\n \nFor ranks, bronze is greater than silver
    which is greater than gold. Along with sort=rank, set max=gold for just gold badges,
    max=silver&min=silver for just silver, and min=bronze for just bronze.\n \nrank
    is the default sort.\n \n{ids} can contain up to 100 semicolon delimited ids,
    to find ids programatically look for user_id on user or shallow_user objects.\n
    \nThis method returns a list of badges."
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/253-stack-exchange.jpg
  humanURL: http://stackexchange.com
  baseURL: https://api.stackexchange.com//2.2//users/{ids}/badges
  tags: Users,Badges
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/users/master/_listings/stack-exchange/usersidsbadges-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/users/master/_listings/stack-exchange/usersidsbadges-get-openapi.md
- name: Stack Exchange Get User Comments
  x-api-slug: stack-exchange
  description: "Get the comments posted by users in {ids}.\n \n{ids} can contain up
    to 100 semicolon delimited ids, to find ids programatically look for user_id on
    user or shallow_user objects.\n \nThe sorts accepted by this method operate on
    the follow fields of the comment object:\n - creation - creation_date\n - votes
    - score\n  creation is the default sort.\n \n It is possible to create moderately
    complex queries using sort, min, max, fromdate, and todate.\n \nThis method returns
    a list of comments."
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/253-stack-exchange.jpg
  humanURL: http://stackexchange.com
  baseURL: https://api.stackexchange.com//2.2//users/{ids}/comments
  tags: Users,Comments
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/users/master/_listings/stack-exchange/usersidscomments-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/users/master/_listings/stack-exchange/usersidscomments-get-openapi.md
- name: Stack Exchange Get User Comments Told
  x-api-slug: stack-exchange
  description: "Get the comments that the users in {ids} have posted in reply to the
    single user identified in {toid}.\n \nThis method is useful for extracting conversations,
    especially over time or across multiple posts.\n \n{ids} can contain up to 100
    semicolon delimited ids, to find ids programatically look for user_id on user
    or shallow_user objects. {toid} can contain only 1 id, found in the same manner
    as those in {ids}.\n \nThe sorts accepted by this method operate on the follow
    fields of the comment object:\n - creation - creation_date\n - votes - score\n
    \ creation is the default sort.\n \n It is possible to create moderately complex
    queries using sort, min, max, fromdate, and todate.\n \nThis method returns a
    list of comments."
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/253-stack-exchange.jpg
  humanURL: http://stackexchange.com
  baseURL: https://api.stackexchange.com//2.2//users/{ids}/comments/{toid}
  tags: Users,Comments
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/users/master/_listings/stack-exchange/usersidscommentstoid-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/users/master/_listings/stack-exchange/usersidscommentstoid-get-openapi.md
- name: Stack Exchange Get User Favorites
  x-api-slug: stack-exchange
  description: "Get the questions that users in {ids} have favorited.\n \nThis method
    is effectively a view onto a user's favorites tab.\n \n{ids} can contain up to
    100 semicolon delimited ids, to find ids programatically look for user_id on user
    or shallow_user objects.\n \nThe sorts accepted by this method operate on the
    follow fields of the question object:\n - activity - last_activity_date\n - creation
    - creation_date\n - votes - score\n - added - when the user favorited the question\n
    \ activity is the default sort.\n \n It is possible to create moderately complex
    queries using sort, min, max, fromdate, and todate.\n \nThis method returns a
    list of questions."
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/253-stack-exchange.jpg
  humanURL: http://stackexchange.com
  baseURL: https://api.stackexchange.com//2.2//users/{ids}/favorites
  tags: Users,Favorites
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/users/master/_listings/stack-exchange/usersidsfavorites-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/users/master/_listings/stack-exchange/usersidsfavorites-get-openapi.md
- name: Stack Exchange Get User Mentioned
  x-api-slug: stack-exchange
  description: "Gets all the comments that the users in {ids} were mentioned in.\n
    \nNote, to count as a mention the comment must be considered to be \"in reply
    to\" a user. Most importantly, this means that a comment can only be in reply
    to a single user.\n \n{ids} can contain up to 100 semicolon delimited ids, to
    find ids programatically look for user_id on user or shallow_user objects.\n \nThe
    sorts accepted by this method operate on the follow fields of the comment object:\n
    - creation - creation_date\n - votes - score\n  It is possible to create moderately
    complex queries using sort, min, max, fromdate, and todate.\n \nThis method returns
    a list of comments."
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/253-stack-exchange.jpg
  humanURL: http://stackexchange.com
  baseURL: https://api.stackexchange.com//2.2//users/{ids}/mentioned
  tags: Users,Mentioned
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/users/master/_listings/stack-exchange/usersidsmentioned-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/users/master/_listings/stack-exchange/usersidsmentioned-get-openapi.md
- name: Stack Exchange Get User Merges
  x-api-slug: stack-exchange
  description: "Returns a record of merges that have occurred involving the passed
    account ids.\n \nThis method allows you to take now invalid account ids and find
    what account they've become, or take currently valid account ids and find which
    ids were equivalent in the past.\n \nThis is most useful when confirming that
    an account_id is in fact \"new\" to an application.\n \nAccount merges can happen
    for a wide range of reasons, applications should not make assumptions that merges
    have particular causes.\n \nNote that accounts are managed at a network level,
    users on a site may be merged due to an account level merge but there is no guarantee
    that a merge has an effect on any particular site.\n \nThis method returns a list
    of account_merge."
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/253-stack-exchange.jpg
  humanURL: http://stackexchange.com
  baseURL: https://api.stackexchange.com//2.2//users/{ids}/merges
  tags: Users,Merges
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/users/master/_listings/stack-exchange/usersidsmerges-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/users/master/_listings/stack-exchange/usersidsmerges-get-openapi.md
- name: Stack Exchange Get User Questions
  x-api-slug: stack-exchange
  description: "Gets the questions asked by the users in {ids}.\n \n{ids} can contain
    up to 100 semicolon delimited ids, to find ids programatically look for user_id
    on user or shallow_user objects.\n \nThe sorts accepted by this method operate
    on the follow fields of the question object:\n - activity - last_activity_date\n
    - creation - creation_date\n - votes - score\n  activity is the default sort.\n
    \n It is possible to create moderately complex queries using sort, min, max, fromdate,
    and todate.\n \nThis method returns a list of questions."
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/253-stack-exchange.jpg
  humanURL: http://stackexchange.com
  baseURL: https://api.stackexchange.com//2.2//users/{ids}/questions
  tags: Users,Questions
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/users/master/_listings/stack-exchange/usersidsquestions-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/users/master/_listings/stack-exchange/usersidsquestions-get-openapi.md
- name: Stack Exchange Get User Questions Featured
  x-api-slug: stack-exchange
  description: "Gets the questions on which the users in {ids} have active bounties.\n
    \n{ids} can contain up to 100 semicolon delimited ids, to find ids programatically
    look for user_id on user or shallow_user objects.\n \nThe sorts accepted by this
    method operate on the follow fields of the question object:\n - activity - last_activity_date\n
    - creation - creation_date\n - votes - score\n  activity is the default sort.\n
    \n It is possible to create moderately complex queries using sort, min, max, fromdate,
    and todate.\n \nThis method returns a list of questions."
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/253-stack-exchange.jpg
  humanURL: http://stackexchange.com
  baseURL: https://api.stackexchange.com//2.2//users/{ids}/questions/featured
  tags: Users,Featured
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/users/master/_listings/stack-exchange/usersidsquestionsfeatured-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/users/master/_listings/stack-exchange/usersidsquestionsfeatured-get-openapi.md
- name: Stack Exchange Get User Questions No Answers
  x-api-slug: stack-exchange
  description: "Gets the questions asked by the users in {ids} which have no answers.\n
    \nQuestions returns by this method actually have zero undeleted answers. It is
    completely disjoint /users/{ids}/questions/unanswered and /users/{ids}/questions/unaccepted,
    which only return questions with at least one answer, subject to other contraints.\n
    \n{ids} can contain up to 100 semicolon delimited ids, to find ids programatically
    look for user_id on user or shallow_user objects.\n \nThe sorts accepted by this
    method operate on the follow fields of the question object:\n - activity - last_activity_date\n
    - creation - creation_date\n - votes - score\n  activity is the default sort.\n
    \n It is possible to create moderately complex queries using sort, min, max, fromdate,
    and todate.\n \nThis method returns a list of questions."
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/253-stack-exchange.jpg
  humanURL: http://stackexchange.com
  baseURL: https://api.stackexchange.com//2.2//users/{ids}/questions/no-answers
  tags: Users,Answers
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/users/master/_listings/stack-exchange/usersidsquestionsnoanswers-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/users/master/_listings/stack-exchange/usersidsquestionsnoanswers-get-openapi.md
- name: Stack Exchange Get User Questions Unnacepted
  x-api-slug: stack-exchange
  description: "Gets the questions asked by the users in {ids} which have at least
    one answer, but no accepted answer.\n \nQuestions returned by this method have
    answers, but the owner has not opted to accept any of them.\n \n{ids} can contain
    up to 100 semicolon delimited ids, to find ids programatically look for user_id
    on user or shallow_user objects.\n \nThe sorts accepted by this method operate
    on the follow fields of the question object:\n - activity - last_activity_date\n
    - creation - creation_date\n - votes - score\n  activity is the default sort.\n
    \n It is possible to create moderately complex queries using sort, min, max, fromdate,
    and todate.\n \nThis method returns a list of questions."
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/253-stack-exchange.jpg
  humanURL: http://stackexchange.com
  baseURL: https://api.stackexchange.com//2.2//users/{ids}/questions/unaccepted
  tags: Users,Unaccepted
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/users/master/_listings/stack-exchange/usersidsquestionsunaccepted-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/users/master/_listings/stack-exchange/usersidsquestionsunaccepted-get-openapi.md
- name: Stack Exchange Get User Questions Unanswered
  x-api-slug: stack-exchange
  description: "Gets the questions asked by the users in {ids} which the site consideres
    unanswered, while still having at least one answer posted.\n \nThese rules are
    subject to change, but currently any question without at least one upvoted or
    accepted answer is considered unanswered.\n \nTo get the set of questions that
    a user probably considers unanswered, the returned questions should be unioned
    with those returned by /users/{id}/questions/no-answers. These methods are distinct
    so that truly unanswered (that is, zero posted answers) questions can be easily
    separated from mearly poorly or inadequately answered ones.\n \n{ids} can contain
    up to 100 semicolon delimited ids, to find ids programatically look for user_id
    on user or shallow_user objects.\n \nThe sorts accepted by this method operate
    on the follow fields of the question object:\n - activity - last_activity_date\n
    - creation - creation_date\n - votes - score\n  activity is the default sort.\n
    \n It is possible to create moderately complex queries using sort, min, max, fromdate,
    and todate.\n \nThis method returns a list of questions."
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/253-stack-exchange.jpg
  humanURL: http://stackexchange.com
  baseURL: https://api.stackexchange.com//2.2//users/{ids}/questions/unanswered
  tags: Users,Unanswerd
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/users/master/_listings/stack-exchange/usersidsquestionsunanswered-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/users/master/_listings/stack-exchange/usersidsquestionsunanswered-get-openapi.md
- name: Stack Exchange Get User Reputation
  x-api-slug: stack-exchange
  description: "Gets a subset of the reputation changes for users in {ids}.\n \nReputation
    changes are intentionally scrubbed of some data to make it difficult to correlate
    votes on particular posts with user reputation changes. That being said, this
    method returns enough data for reasonable display of reputation trends.\n \n{ids}
    can contain up to 100 semicolon delimited ids, to find ids programatically look
    for user_id on user or shallow_user objects.\n \nThis method returns a list of
    reputation objects."
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/253-stack-exchange.jpg
  humanURL: http://stackexchange.com
  baseURL: https://api.stackexchange.com//2.2//users/{ids}/reputation
  tags: Users,Reputation
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/users/master/_listings/stack-exchange/usersidsreputation-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/users/master/_listings/stack-exchange/usersidsreputation-get-openapi.md
- name: Stack Exchange Get User Reputation History
  x-api-slug: stack-exchange
  description: "Returns users' public reputation history.\n \nThis method returns
    a list of reputation_history."
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/253-stack-exchange.jpg
  humanURL: http://stackexchange.com
  baseURL: https://api.stackexchange.com//2.2//users/{ids}/reputation-history
  tags: Users,Reputation,History
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/users/master/_listings/stack-exchange/usersidsreputationhistory-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/users/master/_listings/stack-exchange/usersidsreputationhistory-get-openapi.md
- name: Stack Exchange Get User Suggested Edits
  x-api-slug: stack-exchange
  description: "Returns the suggested edits a users in {ids} have submitted.\n \n{ids}
    can contain up to 100 semicolon delimited ids, to find ids programatically look
    for user_id on user or shallow_user objects.\n \nThe sorts accepted by this method
    operate on the follow fields of the suggested_edit object:\n - creation - creation_date\n
    - approval - approval_date Does not return unapproved suggested_edits\n - rejection
    - rejection_date Does not return unrejected suggested_edits\n  creation is the
    default sort.\n \n It is possible to create moderately complex queries using sort,
    min, max, fromdate, and todate.\n \nThis method returns a list of suggested-edits."
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/253-stack-exchange.jpg
  humanURL: http://stackexchange.com
  baseURL: https://api.stackexchange.com//2.2//users/{ids}/suggested-edits
  tags: Users,Suggested Edits
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/users/master/_listings/stack-exchange/usersidssuggestededits-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/users/master/_listings/stack-exchange/usersidssuggestededits-get-openapi.md
- name: Stack Exchange Get User Tags
  x-api-slug: stack-exchange
  description: "Returns the tags the users identified in {ids} have been active in.\n
    \nThis route corresponds roughly to user's stats tab, but does not include tag
    scores. A subset of tag scores are available (on a single user basis) in /users/{id}/top-answer-tags
    and /users/{id}/top-question-tags.\n \n{ids} can contain up to 100 semicolon delimited
    ids, to find ids programatically look for user_id on user or shallow_user objects.\n
    \nThe sorts accepted by this method operate on the follow fields of the tag object:\n
    - popular - count\n - activity - the creation_date of the last question asked
    with the tag\n - name - name\n  popular is the default sort.\n \n It is possible
    to create moderately complex queries using sort, min, max, fromdate, and todate.\n
    \nThis method returns a list of tags."
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/253-stack-exchange.jpg
  humanURL: http://stackexchange.com
  baseURL: https://api.stackexchange.com//2.2//users/{ids}/tags
  tags: Users,Tags
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/users/master/_listings/stack-exchange/usersidstags-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/users/master/_listings/stack-exchange/usersidstags-get-openapi.md
- name: Stack Exchange Get User Timeline
  x-api-slug: stack-exchange
  description: "Returns a subset of the actions the users in {ids} have taken on the
    site.\n \nThis method returns users' posts, edits, and earned badges in the order
    they were accomplished. It is possible to filter to just a window of activity
    using the fromdate and todate parameters.\n \n{ids} can contain up to 100 semicolon
    delimited ids, to find ids programatically look for user_id on user or shallow_user
    objects.\n \nThis method returns a list of user timeline objects."
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/253-stack-exchange.jpg
  humanURL: http://stackexchange.com
  baseURL: https://api.stackexchange.com//2.2//users/{ids}/timeline
  tags: Users,Timiline
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/users/master/_listings/stack-exchange/usersidstimeline-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/users/master/_listings/stack-exchange/usersidstimeline-get-openapi.md
- name: Stack Exchange Get User Inbox
  x-api-slug: stack-exchange
  description: "Returns a user's inbox.\n \nThis method requires an access_token,
    with a scope containing \"read_inbox\".\n \nThis method is effectively an alias
    for /inbox. It is provided for consumers who make strong assumptions about operating
    within the context of a single site rather than the Stack Exchange network as
    a whole.\n \n{id} can contain a single id, to find it programatically look for
    user_id on user or shallow_user objects.\n \nThis method returns a list of inbox
    items."
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/253-stack-exchange.jpg
  humanURL: http://stackexchange.com
  baseURL: https://api.stackexchange.com//2.2//users/{id}/inbox
  tags: Users,Email,Inbox
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/users/master/_listings/stack-exchange/usersidinbox-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/users/master/_listings/stack-exchange/usersidinbox-get-openapi.md
- name: Stack Exchange Get User Inbox Unread
  x-api-slug: stack-exchange
  description: "Returns the unread items in a user's inbox.\n \nThis method requires
    an access_token, with a scope containing \"read_inbox\".\n \nThis method is effectively
    an alias for /inbox/unread. It is provided for consumers who make strong assumptions
    about operating within the context of a single site rather than the Stack Exchange
    network as a whole.\n \n{id} can contain a single id, to find it programatically
    look for user_id on user or shallow_user objects.\n \nThis method returns a list
    of inbox items."
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/253-stack-exchange.jpg
  humanURL: http://stackexchange.com
  baseURL: https://api.stackexchange.com//2.2//users/{id}/inbox/unread
  tags: Users,Email,Inbox
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/users/master/_listings/stack-exchange/usersidinboxunread-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/users/master/_listings/stack-exchange/usersidinboxunread-get-openapi.md
- name: Stack Exchange Get User Notifications
  x-api-slug: stack-exchange
  description: "Returns a user's notifications.\n \nThis method requires an access_token,
    with a scope containing \"read_inbox\".\n \nThis method returns a list of notifications."
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/253-stack-exchange.jpg
  humanURL: http://stackexchange.com
  baseURL: https://api.stackexchange.com//2.2//users/{id}/notifications
  tags: Users,Notifications
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/users/master/_listings/stack-exchange/usersidnotifications-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/users/master/_listings/stack-exchange/usersidnotifications-get-openapi.md
- name: Stack Exchange Get User Notifications Unread
  x-api-slug: stack-exchange
  description: "Returns a user's unread notifications.\n \nThis method requires an
    access_token, with a scope containing \"read_inbox\".\n \nThis method returns
    a list of notifications."
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/253-stack-exchange.jpg
  humanURL: http://stackexchange.com
  baseURL: https://api.stackexchange.com//2.2//users/{id}/notifications/unread
  tags: Users,Notifications
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/users/master/_listings/stack-exchange/usersidnotificationsunread-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/users/master/_listings/stack-exchange/usersidnotificationsunread-get-openapi.md
- name: Stack Exchange Get User Preveleges
  x-api-slug: stack-exchange
  description: "Returns the privileges a user has.\n \nApplications are encouraged
    to calculate privileges themselves, without repeated queries to this method. A
    simple check against the results returned by /privileges and user.user_type would
    be sufficient.\n \n{id} can contain only a single, to find it programatically
    look for user_id on user or shallow_user objects.\n \nThis method returns a list
    of privileges."
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/253-stack-exchange.jpg
  humanURL: http://stackexchange.com
  baseURL: https://api.stackexchange.com//2.2//users/{id}/privileges
  tags: Users,Privileges
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/users/master/_listings/stack-exchange/usersidprivileges-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/users/master/_listings/stack-exchange/usersidprivileges-get-openapi.md
- name: Stack Exchange Get User Reputation History Full
  x-api-slug: stack-exchange
  description: "Returns a user's full reputation history, including private events.\n
    \nThis method requires an access_token, with a scope containing \"private_info\".\n
    \nThis method returns a list of reputation_history."
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/253-stack-exchange.jpg
  humanURL: http://stackexchange.com
  baseURL: https://api.stackexchange.com//2.2//users/{id}/reputation-history/full
  tags: Users,Reputation
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/users/master/_listings/stack-exchange/usersidreputationhistoryfull-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/users/master/_listings/stack-exchange/usersidreputationhistoryfull-get-openapi.md
- name: Stack Exchange Get User Tags Top Answers
  x-api-slug: stack-exchange
  description: "Returns the top 30 answers a user has posted in response to questions
    with the given tags.\n \n{id} can contain a single id, to find it programatically
    look for user_id on user or shallow_user objects. {tags} is limited to 5 tags,
    passing more will result in an error.\n \nThe sorts accepted by this method operate
    on the follow fields of the answer object:\n - activity - last_activity_date\n
    - creation - creation_date\n - votes - score\n  activity is the default sort.\n
    \n It is possible to create moderately complex queries using sort, min, max, fromdate,
    and todate.\n \nThis method returns a list of answers."
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/253-stack-exchange.jpg
  humanURL: http://stackexchange.com
  baseURL: https://api.stackexchange.com//2.2//users/{id}/tags/{tags}/top-answers
  tags: Users,Tags,Answers
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/users/master/_listings/stack-exchange/usersidtagstagstopanswers-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/users/master/_listings/stack-exchange/usersidtagstagstopanswers-get-openapi.md
- name: Stack Exchange Get User Tags Top Questions
  x-api-slug: stack-exchange
  description: "Returns the top 30 questions a user has asked with the given tags.\n
    \n{id} can contain a single id, to find it programatically look for user_id on
    user or shallow_user objects. {tags} is limited to 5 tags, passing more will result
    in an error.\n \nThe sorts accepted by this method operate on the follow fields
    of the question object:\n - activity - last_activity_date\n - creation - creation_date\n
    - votes - score\n  activity is the default sort.\n \n It is possible to create
    moderately complex queries using sort, min, max, fromdate, and todate.\n \nThis
    method returns a list of questions."
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/253-stack-exchange.jpg
  humanURL: http://stackexchange.com
  baseURL: https://api.stackexchange.com//2.2//users/{id}/tags/{tags}/top-questions
  tags: Users,Tags,Questions
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/users/master/_listings/stack-exchange/usersidtagstagstopquestions-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/users/master/_listings/stack-exchange/usersidtagstagstopquestions-get-openapi.md
- name: Stack Exchange Get User Top Answers Tags
  x-api-slug: stack-exchange
  description: "Returns a single user's top tags by answer score.\n \nThis a subset
    of the data returned on a user's tags tab.\n \n{id} can contain a single id, to
    find it programatically look for user_id on user or shallow_user objects.\n \nThis
    method returns a list of top_tag objects."
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/253-stack-exchange.jpg
  humanURL: http://stackexchange.com
  baseURL: https://api.stackexchange.com//2.2//users/{id}/top-answer-tags
  tags: Users,Top Answer Tags
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/users/master/_listings/stack-exchange/usersidtopanswertags-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/users/master/_listings/stack-exchange/usersidtopanswertags-get-openapi.md
- name: Stack Exchange Get User Top Question Tags
  x-api-slug: stack-exchange
  description: "Returns a single user's top tags by question score.\n \nThis a subset
    of the data returned on a user's tags tab.\n \n{id} can contain a single id, to
    find it programatically look for user_id on user or shallow_user objects.\n \nThis
    method returns a list of top_tag objects."
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/253-stack-exchange.jpg
  humanURL: http://stackexchange.com
  baseURL: https://api.stackexchange.com//2.2//users/{id}/top-question-tags
  tags: Users,Top Question Tags
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/users/master/_listings/stack-exchange/usersidtopquestiontags-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/users/master/_listings/stack-exchange/usersidtopquestiontags-get-openapi.md
- name: Stack Exchange
  x-api-slug: stack-exchange
  description: After someone asks a question, members of the community propose answers.
    Others vote on those answers. Very quickly, the answers with the most votes rise
    to the top. You don???t have to read through a lot of discussion to find the best
    answer.    Like to...
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/253-stack-exchange.jpg
  humanURL: http://stackexchange.com
  baseURL: https://api.stackexchange.com//2.2
  tags: Users
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/users/master/_listings/stack-exchange/openapi.md
x-common:
- type: x-authentication
  url: https://api.stackexchange.com/docs/authentication
- type: x-base
  url: https://api.stackexchange.com/
- type: x-blog
  url: http://stackexchange.com/blogs
- type: x-blog-rss
  url: http://blog.stackoverflow.com/feed/
- type: x-crunchbase
  url: http://www.crunchbase.com/company/stack-exchange
- type: x-crunchbase
  url: https://crunchbase.com/organization/stack-exchange
- type: x-developer
  url: http://api.stackexchange.com/
- type: x-email
  url: legal@stackexchange.com
- type: x-email
  url: team@stackexchange.com
- type: x-email
  url: team+api@stackexchange.com
- type: x-error-codes
  url: https://api.stackexchange.com/docs/error-handling
- type: x-github
  url: https://github.com/StackExchange
- type: x-javascript-sdk
  url: https://api.stackexchange.com/docs/js-lib
- type: x-privacy
  url: https://stackexchange.com/legal/privacy-policy
- type: x-rate-limits
  url: https://api.stackexchange.com/docs/throttle
- type: x-selfservice-registration
  url: https://stackapps.com/users/login?returnurl=/apps/oauth/register
- type: x-support
  url: https://stackexchange.com/about/contact
- type: x-terms-of-service
  url: http://stackexchange.com/legal/api-terms-of-use
- type: x-twitter
  url: https://twitter.com/StackExchange
- type: x-website
  url: http://stackexchange.com
- type: x-website
  url: https://stackexchange.com/
include: []
maintainers:
- FN: Kin Lane
  x-twitter: apievangelist
  email: info@apievangelist.com
---