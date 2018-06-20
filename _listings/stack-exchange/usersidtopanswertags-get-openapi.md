---
swagger: "2.0"
x-collection-name: Stack Exchange
x-complete: 0
info:
  title: Stack Exchange Get User Top Answers Tags
  description: "Returns a single user's top tags by answer score.\n \nThis a subset
    of the data returned on a user's tags tab.\n \n{id} can contain a single id, to
    find it programatically look for user_id on user or shallow_user objects.\n \nThis
    method returns a list of top_tag objects."
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
  /users/{ids}/questions/unaccepted:
    get:
      summary: Get User Questions Unnacepted
      description: "Gets the questions asked by the users in {ids} which have at least
        one answer, but no accepted answer.\n \nQuestions returned by this method
        have answers, but the owner has not opted to accept any of them.\n \n{ids}
        can contain up to 100 semicolon delimited ids, to find ids programatically
        look for user_id on user or shallow_user objects.\n \nThe sorts accepted by
        this method operate on the follow fields of the question object:\n - activity
        - last_activity_date\n - creation - creation_date\n - votes - score\n  activity
        is the default sort.\n \n It is possible to create moderately complex queries
        using sort, min, max, fromdate, and todate.\n \nThis method returns a list
        of questions."
      operationId: gets-the-questions-asked-by-the-users-in-ids-which-have-at-least-one-answer-but-no-accepted-answer-q
      x-api-path-slug: usersidsquestionsunaccepted-get
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
      - Unaccepted
  /users/{ids}/questions/unanswered:
    get:
      summary: Get User Questions Unanswered
      description: "Gets the questions asked by the users in {ids} which the site
        consideres unanswered, while still having at least one answer posted.\n \nThese
        rules are subject to change, but currently any question without at least one
        upvoted or accepted answer is considered unanswered.\n \nTo get the set of
        questions that a user probably considers unanswered, the returned questions
        should be unioned with those returned by /users/{id}/questions/no-answers.
        These methods are distinct so that truly unanswered (that is, zero posted
        answers) questions can be easily separated from mearly poorly or inadequately
        answered ones.\n \n{ids} can contain up to 100 semicolon delimited ids, to
        find ids programatically look for user_id on user or shallow_user objects.\n
        \nThe sorts accepted by this method operate on the follow fields of the question
        object:\n - activity - last_activity_date\n - creation - creation_date\n -
        votes - score\n  activity is the default sort.\n \n It is possible to create
        moderately complex queries using sort, min, max, fromdate, and todate.\n \nThis
        method returns a list of questions."
      operationId: gets-the-questions-asked-by-the-users-in-ids-which-the-site-consideres-unanswered-while-still-having
      x-api-path-slug: usersidsquestionsunanswered-get
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
      - Unanswerd
  /users/{ids}/reputation:
    get:
      summary: Get User Reputation
      description: "Gets a subset of the reputation changes for users in {ids}.\n
        \nReputation changes are intentionally scrubbed of some data to make it difficult
        to correlate votes on particular posts with user reputation changes. That
        being said, this method returns enough data for reasonable display of reputation
        trends.\n \n{ids} can contain up to 100 semicolon delimited ids, to find ids
        programatically look for user_id on user or shallow_user objects.\n \nThis
        method returns a list of reputation objects."
      operationId: gets-a-subset-of-the-reputation-changes-for-users-in-ids-reputation-changes-are-intentionally-scrubb
      x-api-path-slug: usersidsreputation-get
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
        name: page
      - in: query
        name: pagesize
      - in: query
        name: site
        description: Each of these methods operates on a single site at a time, identified
          by the site parameter
      - in: query
        name: todate
        description: Unix date
      responses:
        200:
          description: OK
      tags:
      - Users
      - Reputation
  /users/{ids}/reputation-history:
    get:
      summary: Get User Reputation History
      description: "Returns users' public reputation history.\n \nThis method returns
        a list of reputation_history."
      operationId: returns-users-public-reputation-history-this-method-returns-a-list-of-reputation-history
      x-api-path-slug: usersidsreputationhistory-get
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
      - in: query
        name: site
        description: Each of these methods operates on a single site at a time, identified
          by the site parameter
      responses:
        200:
          description: OK
      tags:
      - Users
      - Reputation
      - History
  /users/{ids}/suggested-edits:
    get:
      summary: Get User Suggested Edits
      description: "Returns the suggested edits a users in {ids} have submitted.\n
        \n{ids} can contain up to 100 semicolon delimited ids, to find ids programatically
        look for user_id on user or shallow_user objects.\n \nThe sorts accepted by
        this method operate on the follow fields of the suggested_edit object:\n -
        creation - creation_date\n - approval - approval_date Does not return unapproved
        suggested_edits\n - rejection - rejection_date Does not return unrejected
        suggested_edits\n  creation is the default sort.\n \n It is possible to create
        moderately complex queries using sort, min, max, fromdate, and todate.\n \nThis
        method returns a list of suggested-edits."
      operationId: returns-the-suggested-edits-a-users-in-ids-have-submitted-ids-can-contain-up-to-100-semicolon-delimi
      x-api-path-slug: usersidssuggestededits-get
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
        description: sort = creation => datesort = approval => datesort = rejection
          => date
      - in: query
        name: min
        description: sort = creation => datesort = approval => datesort = rejection
          => date
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
      - Suggested Edits
  /users/{ids}/tags:
    get:
      summary: Get User Tags
      description: "Returns the tags the users identified in {ids} have been active
        in.\n \nThis route corresponds roughly to user's stats tab, but does not include
        tag scores. A subset of tag scores are available (on a single user basis)
        in /users/{id}/top-answer-tags and /users/{id}/top-question-tags.\n \n{ids}
        can contain up to 100 semicolon delimited ids, to find ids programatically
        look for user_id on user or shallow_user objects.\n \nThe sorts accepted by
        this method operate on the follow fields of the tag object:\n - popular -
        count\n - activity - the creation_date of the last question asked with the
        tag\n - name - name\n  popular is the default sort.\n \n It is possible to
        create moderately complex queries using sort, min, max, fromdate, and todate.\n
        \nThis method returns a list of tags."
      operationId: returns-the-tags-the-users-identified-in-ids-have-been-active-in-this-route-corresponds-roughly-to-u
      x-api-path-slug: usersidstags-get
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
        description: sort = popular => numbersort = activity => datesort = name =>
          string
      - in: query
        name: min
        description: sort = popular => numbersort = activity => datesort = name =>
          string
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
      - Tags
  /users/{ids}/timeline:
    get:
      summary: Get User Timeline
      description: "Returns a subset of the actions the users in {ids} have taken
        on the site.\n \nThis method returns users' posts, edits, and earned badges
        in the order they were accomplished. It is possible to filter to just a window
        of activity using the fromdate and todate parameters.\n \n{ids} can contain
        up to 100 semicolon delimited ids, to find ids programatically look for user_id
        on user or shallow_user objects.\n \nThis method returns a list of user timeline
        objects."
      operationId: returns-a-subset-of-the-actions-the-users-in-ids-have-taken-on-the-site-this-method-returns-users-po
      x-api-path-slug: usersidstimeline-get
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
        name: page
      - in: query
        name: pagesize
      - in: query
        name: site
        description: Each of these methods operates on a single site at a time, identified
          by the site parameter
      - in: query
        name: todate
        description: Unix date
      responses:
        200:
          description: OK
      tags:
      - Users
      - Timiline
  /users/{id}/inbox:
    get:
      summary: Get User Inbox
      description: "Returns a user's inbox.\n \nThis method requires an access_token,
        with a scope containing \"read_inbox\".\n \nThis method is effectively an
        alias for /inbox. It is provided for consumers who make strong assumptions
        about operating within the context of a single site rather than the Stack
        Exchange network as a whole.\n \n{id} can contain a single id, to find it
        programatically look for user_id on user or shallow_user objects.\n \nThis
        method returns a list of inbox items."
      operationId: returns-a-users-inbox-this-method-requires-an-access-token-with-a-scope-containing-read-inbox-this-m
      x-api-path-slug: usersidinbox-get
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
        name: id
      - in: query
        name: page
      - in: query
        name: pagesize
      - in: query
        name: site
        description: Each of these methods operates on a single site at a time, identified
          by the site parameter
      responses:
        200:
          description: OK
      tags:
      - Users
      - Email
      - Inbox
  /users/{id}/inbox/unread:
    get:
      summary: Get User Inbox Unread
      description: "Returns the unread items in a user's inbox.\n \nThis method requires
        an access_token, with a scope containing \"read_inbox\".\n \nThis method is
        effectively an alias for /inbox/unread. It is provided for consumers who make
        strong assumptions about operating within the context of a single site rather
        than the Stack Exchange network as a whole.\n \n{id} can contain a single
        id, to find it programatically look for user_id on user or shallow_user objects.\n
        \nThis method returns a list of inbox items."
      operationId: returns-the-unread-items-in-a-users-inbox-this-method-requires-an-access-token-with-a-scope-containi
      x-api-path-slug: usersidinboxunread-get
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
        name: id
      - in: query
        name: page
      - in: query
        name: pagesize
      - in: query
        name: since
        description: Unix date
      - in: query
        name: site
        description: Each of these methods operates on a single site at a time, identified
          by the site parameter
      responses:
        200:
          description: OK
      tags:
      - Users
      - Email
      - Inbox
  /users/{id}/notifications:
    get:
      summary: Get User Notifications
      description: "Returns a user's notifications.\n \nThis method requires an access_token,
        with a scope containing \"read_inbox\".\n \nThis method returns a list of
        notifications."
      operationId: returns-a-users-notifications-this-method-requires-an-access-token-with-a-scope-containing-read-inbo
      x-api-path-slug: usersidnotifications-get
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
        name: id
      - in: query
        name: page
      - in: query
        name: pagesize
      - in: query
        name: site
        description: Each of these methods operates on a single site at a time, identified
          by the site parameter
      responses:
        200:
          description: OK
      tags:
      - Users
      - Notifications
  /users/{id}/notifications/unread:
    get:
      summary: Get User Notifications Unread
      description: "Returns a user's unread notifications.\n \nThis method requires
        an access_token, with a scope containing \"read_inbox\".\n \nThis method returns
        a list of notifications."
      operationId: returns-a-users-unread-notifications-this-method-requires-an-access-token-with-a-scope-containing-re
      x-api-path-slug: usersidnotificationsunread-get
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
        name: id
      - in: query
        name: page
      - in: query
        name: pagesize
      - in: query
        name: site
        description: Each of these methods operates on a single site at a time, identified
          by the site parameter
      responses:
        200:
          description: OK
      tags:
      - Users
      - Notifications
  /users/{id}/privileges:
    get:
      summary: Get User Preveleges
      description: "Returns the privileges a user has.\n \nApplications are encouraged
        to calculate privileges themselves, without repeated queries to this method.
        A simple check against the results returned by /privileges and user.user_type
        would be sufficient.\n \n{id} can contain only a single, to find it programatically
        look for user_id on user or shallow_user objects.\n \nThis method returns
        a list of privileges."
      operationId: returns-the-privileges-a-user-has-applications-are-encouraged-to-calculate-privileges-themselves-wit
      x-api-path-slug: usersidprivileges-get
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
        name: id
      - in: query
        name: page
      - in: query
        name: pagesize
      - in: query
        name: site
        description: Each of these methods operates on a single site at a time, identified
          by the site parameter
      responses:
        200:
          description: OK
      tags:
      - Users
      - Privileges
  /users/{id}/reputation-history/full:
    get:
      summary: Get User Reputation History Full
      description: "Returns a user's full reputation history, including private events.\n
        \nThis method requires an access_token, with a scope containing \"private_info\".\n
        \nThis method returns a list of reputation_history."
      operationId: returns-a-users-full-reputation-history-including-private-events-this-method-requires-an-access-toke
      x-api-path-slug: usersidreputationhistoryfull-get
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
        name: id
      - in: query
        name: page
      - in: query
        name: pagesize
      - in: query
        name: site
        description: Each of these methods operates on a single site at a time, identified
          by the site parameter
      responses:
        200:
          description: OK
      tags:
      - Users
      - Reputation
  /users/{id}/tags/{tags}/top-answers:
    get:
      summary: Get User Tags Top Answers
      description: "Returns the top 30 answers a user has posted in response to questions
        with the given tags.\n \n{id} can contain a single id, to find it programatically
        look for user_id on user or shallow_user objects. {tags} is limited to 5 tags,
        passing more will result in an error.\n \nThe sorts accepted by this method
        operate on the follow fields of the answer object:\n - activity - last_activity_date\n
        - creation - creation_date\n - votes - score\n  activity is the default sort.\n
        \n It is possible to create moderately complex queries using sort, min, max,
        fromdate, and todate.\n \nThis method returns a list of answers."
      operationId: returns-the-top-30-answers-a-user-has-posted-in-response-to-questions-with-the-given-tags-id-can-con
      x-api-path-slug: usersidtagstagstopanswers-get
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
        name: id
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
      - in: path
        name: tags
        description: String list (semicolon delimited)
      - in: query
        name: todate
        description: Unix date
      responses:
        200:
          description: OK
      tags:
      - Users
      - Tags
      - Answers
  /users/{id}/tags/{tags}/top-questions:
    get:
      summary: Get User Tags Top Questions
      description: "Returns the top 30 questions a user has asked with the given tags.\n
        \n{id} can contain a single id, to find it programatically look for user_id
        on user or shallow_user objects. {tags} is limited to 5 tags, passing more
        will result in an error.\n \nThe sorts accepted by this method operate on
        the follow fields of the question object:\n - activity - last_activity_date\n
        - creation - creation_date\n - votes - score\n  activity is the default sort.\n
        \n It is possible to create moderately complex queries using sort, min, max,
        fromdate, and todate.\n \nThis method returns a list of questions."
      operationId: returns-the-top-30-questions-a-user-has-asked-with-the-given-tags-id-can-contain-a-single-id-to-find
      x-api-path-slug: usersidtagstagstopquestions-get
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
        name: id
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
      - in: path
        name: tags
        description: String list (semicolon delimited)
      - in: query
        name: todate
        description: Unix date
      responses:
        200:
          description: OK
      tags:
      - Users
      - Tags
      - Questions
  /users/{id}/top-answer-tags:
    get:
      summary: Get User Top Answers Tags
      description: "Returns a single user's top tags by answer score.\n \nThis a subset
        of the data returned on a user's tags tab.\n \n{id} can contain a single id,
        to find it programatically look for user_id on user or shallow_user objects.\n
        \nThis method returns a list of top_tag objects."
      operationId: returns-a-single-users-top-tags-by-answer-score-this-a-subset-of-the-data-returned-on-a-users-tags-t
      x-api-path-slug: usersidtopanswertags-get
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
        name: id
      - in: query
        name: page
      - in: query
        name: pagesize
      - in: query
        name: site
        description: Each of these methods operates on a single site at a time, identified
          by the site parameter
      responses:
        200:
          description: OK
      tags:
      - Users
      - Top Answer Tags
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