---
swagger: "2.0"
x-collection-name: Stack Exchange
x-complete: 0
info:
  title: Stack Exchange Get User Questions No Answers
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
  version: "2.0"
host: api.stackexchange.com
basePath: /2.2
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /users:
    get:
      summary: Get Users
      description: "Returns all users on a site.\n \nThis method returns a list of
        users.\n \nThe sorts accepted by this method operate on the follow fields
        of the user object:\n - reputation - reputation\n - creation - creation_date\n
        - name - display_name\n - modified - last_modified_date\n  reputation is the
        default sort.\n \n It is possible to create moderately complex queries using
        sort, min, max, fromdate, and todate.\n \nThe inname parameter lets consumers
        filter the results down to just those users with a certain substring in their
        display name. For example, inname=kevin will return all users with both users
        named simply \"Kevin\" or those with Kevin as one of (or part of) their names;
        such as \"Kevin Montrose\"."
      operationId: returns-all-users-on-a-site-this-method-returns-a-list-of-users-the-sorts-accepted-by-this-method-op
      x-api-path-slug: users-get
      parameters:
      - in: query
        name: callback
        description: All API responses are JSON, we do support JSONP with the callback
          query parameter
      - in: query
        name: filter
        description: '#DiscussionThe Stack Exchange API allows applications to exclude
          almost every field returned'
      - in: query
        name: fromdate
        description: Unix date
      - in: query
        name: inname
      - in: query
        name: max
        description: sort = reputation => numbersort = creation => datesort = name
          => stringsort = modified => date
      - in: query
        name: min
        description: sort = reputation => numbersort = creation => datesort = name
          => stringsort = modified => date
      - in: query
        name: order
      - in: query
        name: page
      - in: query
        name: pagesize
      - in: query
        name: site
        description: Each of these methods operates on a single site at a time, identified
          by the site parameter
      - in: query
        name: sort
      - in: query
        name: todate
        description: Unix date
      responses:
        200:
          description: OK
      tags:
      - Users
  /users/moderators:
    get:
      summary: Get User Moderators
      description: "Gets those users on a site who can exercise moderation powers.\n
        \nNote, employees of Stack Exchange Inc. will be returned if they have been
        granted moderation powers on a site even if they have never been appointed
        or elected explicitly. This method checks abilities, not the manner in which
        they were obtained.\n \nThe sorts accepted by this method operate on the follow
        fields of the user object:\n - reputation - reputation\n - creation - creation_date\n
        - name - display_name\n - modified - last_modified_date\n  reputation is the
        default sort.\n \n It is possible to create moderately complex queries using
        sort, min, max, fromdate, and todate.\n \nThis method returns a list of users."
      operationId: gets-those-users-on-a-site-who-can-exercise-moderation-powers-note-employees-of-stack-exchange-inc-w
      x-api-path-slug: usersmoderators-get
      parameters:
      - in: query
        name: callback
        description: All API responses are JSON, we do support JSONP with the callback
          query parameter
      - in: query
        name: filter
        description: '#DiscussionThe Stack Exchange API allows applications to exclude
          almost every field returned'
      - in: query
        name: fromdate
        description: Unix date
      - in: query
        name: max
        description: sort = reputation => numbersort = creation => datesort = name
          => stringsort = modified => date
      - in: query
        name: min
        description: sort = reputation => numbersort = creation => datesort = name
          => stringsort = modified => date
      - in: query
        name: order
      - in: query
        name: page
      - in: query
        name: pagesize
      - in: query
        name: site
        description: Each of these methods operates on a single site at a time, identified
          by the site parameter
      - in: query
        name: sort
      - in: query
        name: todate
        description: Unix date
      responses:
        200:
          description: OK
      tags:
      - Users
      - Moderators
  /users/moderators/elected:
    get:
      summary: Get Users Moderators Elected
      description: "Returns those users on a site who both have moderator powers,
        and were actually elected.\n \nThis method excludes Stack Exchange Inc. employees,
        unless they were actually elected moderators on a site (which can only have
        happened prior to their employment).\n \nThe sorts accepted by this method
        operate on the follow fields of the user object:\n - reputation - reputation\n
        - creation - creation_date\n - name - display_name\n - modified - last_modified_date\n
        \ reputation is the default sort.\n \n It is possible to create moderately
        complex queries using sort, min, max, fromdate, and todate.\n \nThis method
        returns a list of users."
      operationId: returns-those-users-on-a-site-who-both-have-moderator-powers-and-were-actually-elected-this-method-e
      x-api-path-slug: usersmoderatorselected-get
      parameters:
      - in: query
        name: callback
        description: All API responses are JSON, we do support JSONP with the callback
          query parameter
      - in: query
        name: filter
        description: '#DiscussionThe Stack Exchange API allows applications to exclude
          almost every field returned'
      - in: query
        name: fromdate
        description: Unix date
      - in: query
        name: max
        description: sort = reputation => numbersort = creation => datesort = name
          => stringsort = modified => date
      - in: query
        name: min
        description: sort = reputation => numbersort = creation => datesort = name
          => stringsort = modified => date
      - in: query
        name: order
      - in: query
        name: page
      - in: query
        name: pagesize
      - in: query
        name: site
        description: Each of these methods operates on a single site at a time, identified
          by the site parameter
      - in: query
        name: sort
      - in: query
        name: todate
        description: Unix date
      responses:
        200:
          description: OK
      tags:
      - Users
      - Moderators
  /users/{ids}:
    get:
      summary: Get User
      description: "Gets the users identified in ids in {ids}.\n \nTypically this
        method will be called to fetch user profiles when you have obtained user ids
        from some other source, such as /questions.\n \n{ids} can contain up to 100
        semicolon delimited ids, to find ids programatically look for user_id on user
        or shallow_user objects.\n \nThe sorts accepted by this method operate on
        the follow fields of the user object:\n - reputation - reputation\n - creation
        - creation_date\n - name - display_name\n - modified - last_modified_date\n
        \ reputation is the default sort.\n \n It is possible to create moderately
        complex queries using sort, min, max, fromdate, and todate.\n \nThis method
        returns a list of users."
      operationId: gets-the-users-identified-in-ids-in-ids-typically-this-method-will-be-called-to-fetch-user-profiles-
      x-api-path-slug: usersids-get
      parameters:
      - in: query
        name: callback
        description: All API responses are JSON, we do support JSONP with the callback
          query parameter
      - in: query
        name: filter
        description: '#DiscussionThe Stack Exchange API allows applications to exclude
          almost every field returned'
      - in: query
        name: fromdate
        description: Unix date
      - in: path
        name: ids
        description: Number list (semicolon delimited)
      - in: query
        name: max
        description: sort = reputation => numbersort = creation => datesort = name
          => stringsort = modified => date
      - in: query
        name: min
        description: sort = reputation => numbersort = creation => datesort = name
          => stringsort = modified => date
      - in: query
        name: order
      - in: query
        name: page
      - in: query
        name: pagesize
      - in: query
        name: site
        description: Each of these methods operates on a single site at a time, identified
          by the site parameter
      - in: query
        name: sort
      - in: query
        name: todate
        description: Unix date
      responses:
        200:
          description: OK
      tags:
      - Users
  /users/{ids}/answers:
    get:
      summary: Get User Answers
      description: "Returns the answers the users in {ids} have posted.\n \n{ids}
        can contain up to 100 semicolon delimited ids, to find ids programatically
        look for user_id on user or shallow_user objects.\n \nThe sorts accepted by
        this method operate on the follow fields of the answer object:\n - activity
        - last_activity_date\n - creation - creation_date\n - votes - score\n  activity
        is the default sort.\n \n It is possible to create moderately complex queries
        using sort, min, max, fromdate, and todate.\n \nThis method returns a list
        of answers."
      operationId: returns-the-answers-the-users-in-ids-have-posted-ids-can-contain-up-to-100-semicolon-delimited-ids-t
      x-api-path-slug: usersidsanswers-get
      parameters:
      - in: query
        name: callback
        description: All API responses are JSON, we do support JSONP with the callback
          query parameter
      - in: query
        name: filter
        description: '#DiscussionThe Stack Exchange API allows applications to exclude
          almost every field returned'
      - in: query
        name: fromdate
        description: Unix date
      - in: path
        name: ids
        description: Number list (semicolon delimited)
      - in: query
        name: max
        description: sort = activity => datesort = creation => datesort = votes =>
          number
      - in: query
        name: min
        description: sort = activity => datesort = creation => datesort = votes =>
          number
      - in: query
        name: order
      - in: query
        name: page
      - in: query
        name: pagesize
      - in: query
        name: site
        description: Each of these methods operates on a single site at a time, identified
          by the site parameter
      - in: query
        name: sort
      - in: query
        name: todate
        description: Unix date
      responses:
        200:
          description: OK
      tags:
      - Users
      - Answers
  /users/{ids}/associated:
    get:
      summary: Get User Associated
      description: "Returns all of a user's associated accounts, given their account_ids
        in {ids}.\n \n{ids} can contain up to 100 semicolon delimited ids, to find
        ids programatically look for account_id on user objects.\n \nThis method returns
        a list of network_users."
      operationId: returns-all-of-a-users-associated-accounts-given-their-account-ids-in-ids-ids-can-contain-up-to-100-
      x-api-path-slug: usersidsassociated-get
      parameters:
      - in: query
        name: callback
        description: All API responses are JSON, we do support JSONP with the callback
          query parameter
      - in: query
        name: filter
        description: '#DiscussionThe Stack Exchange API allows applications to exclude
          almost every field returned'
      - in: path
        name: ids
        description: Number list (semicolon delimited)
      - in: query
        name: page
      - in: query
        name: pagesize
      responses:
        200:
          description: OK
      tags:
      - Users
      - Associated
  /users/{ids}/badges:
    get:
      summary: Get User Badges
      description: "Get the badges the users in {ids} have earned.\n \nBadge sorts
        are a tad complicated. For the purposes of sorting (and min/max) tag_based
        is considered to be greater than named.\n \nThis means that you can get a
        list of all tag based badges a user has by passing min=tag_based, and conversely
        all the named badges by passing max=named, with sort=type.\n \nFor ranks,
        bronze is greater than silver which is greater than gold. Along with sort=rank,
        set max=gold for just gold badges, max=silver&min=silver for just silver,
        and min=bronze for just bronze.\n \nrank is the default sort.\n \n{ids} can
        contain up to 100 semicolon delimited ids, to find ids programatically look
        for user_id on user or shallow_user objects.\n \nThis method returns a list
        of badges."
      operationId: get-the-badges-the-users-in-ids-have-earned-badge-sorts-are-a-tad-complicated-for-the-purposes-of-so
      x-api-path-slug: usersidsbadges-get
      parameters:
      - in: query
        name: callback
        description: All API responses are JSON, we do support JSONP with the callback
          query parameter
      - in: query
        name: filter
        description: '#DiscussionThe Stack Exchange API allows applications to exclude
          almost every field returned'
      - in: query
        name: fromdate
        description: Unix date
      - in: path
        name: ids
        description: Number list (semicolon delimited)
      - in: query
        name: max
        description: sort = rank => stringsort = name => stringsort = type => stringsort
          = awarded => date
      - in: query
        name: min
        description: sort = rank => stringsort = name => stringsort = type => stringsort
          = awarded => date
      - in: query
        name: order
      - in: query
        name: page
      - in: query
        name: pagesize
      - in: query
        name: site
        description: Each of these methods operates on a single site at a time, identified
          by the site parameter
      - in: query
        name: sort
      - in: query
        name: todate
        description: Unix date
      responses:
        200:
          description: OK
      tags:
      - Users
      - Badges
  /users/{ids}/comments:
    get:
      summary: Get User Comments
      description: "Get the comments posted by users in {ids}.\n \n{ids} can contain
        up to 100 semicolon delimited ids, to find ids programatically look for user_id
        on user or shallow_user objects.\n \nThe sorts accepted by this method operate
        on the follow fields of the comment object:\n - creation - creation_date\n
        - votes - score\n  creation is the default sort.\n \n It is possible to create
        moderately complex queries using sort, min, max, fromdate, and todate.\n \nThis
        method returns a list of comments."
      operationId: get-the-comments-posted-by-users-in-ids-ids-can-contain-up-to-100-semicolon-delimited-ids-to-find-id
      x-api-path-slug: usersidscomments-get
      parameters:
      - in: query
        name: callback
        description: All API responses are JSON, we do support JSONP with the callback
          query parameter
      - in: query
        name: filter
        description: '#DiscussionThe Stack Exchange API allows applications to exclude
          almost every field returned'
      - in: query
        name: fromdate
        description: Unix date
      - in: path
        name: ids
        description: Number list (semicolon delimited)
      - in: query
        name: max
        description: sort = creation => datesort = votes => number
      - in: query
        name: min
        description: sort = creation => datesort = votes => number
      - in: query
        name: order
      - in: query
        name: page
      - in: query
        name: pagesize
      - in: query
        name: site
        description: Each of these methods operates on a single site at a time, identified
          by the site parameter
      - in: query
        name: sort
      - in: query
        name: todate
        description: Unix date
      responses:
        200:
          description: OK
      tags:
      - Users
      - Comments
  /users/{ids}/comments/{toid}:
    get:
      summary: Get User Comments Told
      description: "Get the comments that the users in {ids} have posted in reply
        to the single user identified in {toid}.\n \nThis method is useful for extracting
        conversations, especially over time or across multiple posts.\n \n{ids} can
        contain up to 100 semicolon delimited ids, to find ids programatically look
        for user_id on user or shallow_user objects. {toid} can contain only 1 id,
        found in the same manner as those in {ids}.\n \nThe sorts accepted by this
        method operate on the follow fields of the comment object:\n - creation -
        creation_date\n - votes - score\n  creation is the default sort.\n \n It is
        possible to create moderately complex queries using sort, min, max, fromdate,
        and todate.\n \nThis method returns a list of comments."
      operationId: get-the-comments-that-the-users-in-ids-have-posted-in-reply-to-the-single-user-identified-in-toid-th
      x-api-path-slug: usersidscommentstoid-get
      parameters:
      - in: query
        name: callback
        description: All API responses are JSON, we do support JSONP with the callback
          query parameter
      - in: query
        name: filter
        description: '#DiscussionThe Stack Exchange API allows applications to exclude
          almost every field returned'
      - in: query
        name: fromdate
        description: Unix date
      - in: path
        name: ids
        description: Number list (semicolon delimited)
      - in: query
        name: max
        description: sort = creation => datesort = votes => number
      - in: query
        name: min
        description: sort = creation => datesort = votes => number
      - in: query
        name: order
      - in: query
        name: page
      - in: query
        name: pagesize
      - in: query
        name: site
        description: Each of these methods operates on a single site at a time, identified
          by the site parameter
      - in: query
        name: sort
      - in: query
        name: todate
        description: Unix date
      - in: path
        name: toid
      responses:
        200:
          description: OK
      tags:
      - Users
      - Comments
  /users/{ids}/favorites:
    get:
      summary: Get User Favorites
      description: "Get the questions that users in {ids} have favorited.\n \nThis
        method is effectively a view onto a user's favorites tab.\n \n{ids} can contain
        up to 100 semicolon delimited ids, to find ids programatically look for user_id
        on user or shallow_user objects.\n \nThe sorts accepted by this method operate
        on the follow fields of the question object:\n - activity - last_activity_date\n
        - creation - creation_date\n - votes - score\n - added - when the user favorited
        the question\n  activity is the default sort.\n \n It is possible to create
        moderately complex queries using sort, min, max, fromdate, and todate.\n \nThis
        method returns a list of questions."
      operationId: get-the-questions-that-users-in-ids-have-favorited-this-method-is-effectively-a-view-onto-a-users-fa
      x-api-path-slug: usersidsfavorites-get
      parameters:
      - in: query
        name: callback
        description: All API responses are JSON, we do support JSONP with the callback
          query parameter
      - in: query
        name: filter
        description: '#DiscussionThe Stack Exchange API allows applications to exclude
          almost every field returned'
      - in: query
        name: fromdate
        description: Unix date
      - in: path
        name: ids
        description: Number list (semicolon delimited)
      - in: query
        name: max
        description: sort = activity => datesort = creation => datesort = votes =>
          numbersort = added => date
      - in: query
        name: min
        description: sort = activity => datesort = creation => datesort = votes =>
          numbersort = added => date
      - in: query
        name: order
      - in: query
        name: page
      - in: query
        name: pagesize
      - in: query
        name: site
        description: Each of these methods operates on a single site at a time, identified
          by the site parameter
      - in: query
        name: sort
      - in: query
        name: todate
        description: Unix date
      responses:
        200:
          description: OK
      tags:
      - Users
      - Favorites
  /users/{ids}/mentioned:
    get:
      summary: Get User Mentioned
      description: "Gets all the comments that the users in {ids} were mentioned in.\n
        \nNote, to count as a mention the comment must be considered to be \"in reply
        to\" a user. Most importantly, this means that a comment can only be in reply
        to a single user.\n \n{ids} can contain up to 100 semicolon delimited ids,
        to find ids programatically look for user_id on user or shallow_user objects.\n
        \nThe sorts accepted by this method operate on the follow fields of the comment
        object:\n - creation - creation_date\n - votes - score\n  It is possible to
        create moderately complex queries using sort, min, max, fromdate, and todate.\n
        \nThis method returns a list of comments."
      operationId: gets-all-the-comments-that-the-users-in-ids-were-mentioned-in-note-to-count-as-a-mention-the-comment
      x-api-path-slug: usersidsmentioned-get
      parameters:
      - in: query
        name: callback
        description: All API responses are JSON, we do support JSONP with the callback
          query parameter
      - in: query
        name: filter
        description: '#DiscussionThe Stack Exchange API allows applications to exclude
          almost every field returned'
      - in: query
        name: fromdate
        description: Unix date
      - in: path
        name: ids
        description: Number list (semicolon delimited)
      - in: query
        name: max
        description: sort = creation => datesort = votes => number
      - in: query
        name: min
        description: sort = creation => datesort = votes => number
      - in: query
        name: order
      - in: query
        name: page
      - in: query
        name: pagesize
      - in: query
        name: site
        description: Each of these methods operates on a single site at a time, identified
          by the site parameter
      - in: query
        name: sort
      - in: query
        name: todate
        description: Unix date
      responses:
        200:
          description: OK
      tags:
      - Users
      - Mentioned
  /users/{ids}/merges:
    get:
      summary: Get User Merges
      description: "Returns a record of merges that have occurred involving the passed
        account ids.\n \nThis method allows you to take now invalid account ids and
        find what account they've become, or take currently valid account ids and
        find which ids were equivalent in the past.\n \nThis is most useful when confirming
        that an account_id is in fact \"new\" to an application.\n \nAccount merges
        can happen for a wide range of reasons, applications should not make assumptions
        that merges have particular causes.\n \nNote that accounts are managed at
        a network level, users on a site may be merged due to an account level merge
        but there is no guarantee that a merge has an effect on any particular site.\n
        \nThis method returns a list of account_merge."
      operationId: returns-a-record-of-merges-that-have-occurred-involving-the-passed-account-ids-this-method-allows-yo
      x-api-path-slug: usersidsmerges-get
      parameters:
      - in: query
        name: callback
        description: All API responses are JSON, we do support JSONP with the callback
          query parameter
      - in: query
        name: filter
        description: '#DiscussionThe Stack Exchange API allows applications to exclude
          almost every field returned'
      - in: path
        name: ids
        description: Number list (semicolon delimited)
      - in: query
        name: page
      - in: query
        name: pagesize
      responses:
        200:
          description: OK
      tags:
      - Users
      - Merges
  /users/{ids}/questions:
    get:
      summary: Get User Questions
      description: "Gets the questions asked by the users in {ids}.\n \n{ids} can
        contain up to 100 semicolon delimited ids, to find ids programatically look
        for user_id on user or shallow_user objects.\n \nThe sorts accepted by this
        method operate on the follow fields of the question object:\n - activity -
        last_activity_date\n - creation - creation_date\n - votes - score\n  activity
        is the default sort.\n \n It is possible to create moderately complex queries
        using sort, min, max, fromdate, and todate.\n \nThis method returns a list
        of questions."
      operationId: gets-the-questions-asked-by-the-users-in-ids-ids-can-contain-up-to-100-semicolon-delimited-ids-to-fi
      x-api-path-slug: usersidsquestions-get
      parameters:
      - in: query
        name: callback
        description: All API responses are JSON, we do support JSONP with the callback
          query parameter
      - in: query
        name: filter
        description: '#DiscussionThe Stack Exchange API allows applications to exclude
          almost every field returned'
      - in: query
        name: fromdate
        description: Unix date
      - in: path
        name: ids
        description: Number list (semicolon delimited)
      - in: query
        name: max
        description: sort = activity => datesort = creation => datesort = votes =>
          number
      - in: query
        name: min
        description: sort = activity => datesort = creation => datesort = votes =>
          number
      - in: query
        name: order
      - in: query
        name: page
      - in: query
        name: pagesize
      - in: query
        name: site
        description: Each of these methods operates on a single site at a time, identified
          by the site parameter
      - in: query
        name: sort
      - in: query
        name: todate
        description: Unix date
      responses:
        200:
          description: OK
      tags:
      - Users
      - Questions
  /users/{ids}/questions/featured:
    get:
      summary: Get User Questions Featured
      description: "Gets the questions on which the users in {ids} have active bounties.\n
        \n{ids} can contain up to 100 semicolon delimited ids, to find ids programatically
        look for user_id on user or shallow_user objects.\n \nThe sorts accepted by
        this method operate on the follow fields of the question object:\n - activity
        - last_activity_date\n - creation - creation_date\n - votes - score\n  activity
        is the default sort.\n \n It is possible to create moderately complex queries
        using sort, min, max, fromdate, and todate.\n \nThis method returns a list
        of questions."
      operationId: gets-the-questions-on-which-the-users-in-ids-have-active-bounties-ids-can-contain-up-to-100-semicolo
      x-api-path-slug: usersidsquestionsfeatured-get
      parameters:
      - in: query
        name: callback
        description: All API responses are JSON, we do support JSONP with the callback
          query parameter
      - in: query
        name: filter
        description: '#DiscussionThe Stack Exchange API allows applications to exclude
          almost every field returned'
      - in: query
        name: fromdate
        description: Unix date
      - in: path
        name: ids
        description: Number list (semicolon delimited)
      - in: query
        name: max
        description: sort = activity => datesort = creation => datesort = votes =>
          number
      - in: query
        name: min
        description: sort = activity => datesort = creation => datesort = votes =>
          number
      - in: query
        name: order
      - in: query
        name: page
      - in: query
        name: pagesize
      - in: query
        name: site
        description: Each of these methods operates on a single site at a time, identified
          by the site parameter
      - in: query
        name: sort
      - in: query
        name: todate
        description: Unix date
      responses:
        200:
          description: OK
      tags:
      - Users
      - Featured
  /users/{ids}/questions/no-answers:
    get:
      summary: Get User Questions No Answers
      description: "Gets the questions asked by the users in {ids} which have no answers.\n
        \nQuestions returns by this method actually have zero undeleted answers. It
        is completely disjoint /users/{ids}/questions/unanswered and /users/{ids}/questions/unaccepted,
        which only return questions with at least one answer, subject to other contraints.\n
        \n{ids} can contain up to 100 semicolon delimited ids, to find ids programatically
        look for user_id on user or shallow_user objects.\n \nThe sorts accepted by
        this method operate on the follow fields of the question object:\n - activity
        - last_activity_date\n - creation - creation_date\n - votes - score\n  activity
        is the default sort.\n \n It is possible to create moderately complex queries
        using sort, min, max, fromdate, and todate.\n \nThis method returns a list
        of questions."
      operationId: gets-the-questions-asked-by-the-users-in-ids-which-have-no-answers-questions-returns-by-this-method-
      x-api-path-slug: usersidsquestionsnoanswers-get
      parameters:
      - in: query
        name: callback
        description: All API responses are JSON, we do support JSONP with the callback
          query parameter
      - in: query
        name: filter
        description: '#DiscussionThe Stack Exchange API allows applications to exclude
          almost every field returned'
      - in: query
        name: fromdate
        description: Unix date
      - in: path
        name: ids
        description: Number list (semicolon delimited)
      - in: query
        name: max
        description: sort = activity => datesort = creation => datesort = votes =>
          number
      - in: query
        name: min
        description: sort = activity => datesort = creation => datesort = votes =>
          number
      - in: query
        name: order
      - in: query
        name: page
      - in: query
        name: pagesize
      - in: query
        name: site
        description: Each of these methods operates on a single site at a time, identified
          by the site parameter
      - in: query
        name: sort
      - in: query
        name: todate
        description: Unix date
      responses:
        200:
          description: OK
      tags:
      - Users
      - Answers
x-streamrank:
  polling_total_time_average: 0
  polling_size_download_average: 0
  streaming_total_time_average: 0
  streaming_size_download_average: 0
  change_yes: 0
  change_no: 0
  time_percentage: 0
  size_percentage: 0
  change_percentage: 0
  last_run: ""
  days_run: 0
  minute_run: 0
---