---
name: Instructure
x-slug: instructure
description: Instructure makes software that makes smarter people. Products include
  Canvas LMS, Bridge and Canvas Network.
image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/820-instructure.jpg
x-kinRank: "8"
x-alexaRank: "367"
tags: Items
created: "2018-06-20"
modified: "2018-06-20"
url: https://raw.githubusercontent.com/streamdata-gallery-topics/items/master/_listings/instructure/apis.md
specificationVersion: "0.14"
apis:
- name: Instructure Canvas Courses API List module items
  x-api-slug: instructure-canvas-courses-api
  description: List module items.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/820-instructure.jpg
  humanURL: http://instructure.com
  baseURL: https://canvas.instructure.com//api/v1//courses/{course_id}/modules/module_id/items
  tags: Courses,Course,Id,Modules,Module,Id,Items
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/items/master/_listings/instructure/coursescourse-idmodulesmodule-iditems-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/items/master/_listings/instructure/coursescourse-idmodulesmodule-iditems-get-openapi.md
- name: Instructure Canvas Courses API Create a module item
  x-api-slug: instructure-canvas-courses-api
  description: Create a module item.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/820-instructure.jpg
  humanURL: http://instructure.com
  baseURL: https://canvas.instructure.com//api/v1//courses/{course_id}/modules/module_id/items
  tags: Courses,Course,Id,Modules,Module,Id,Items
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/items/master/_listings/instructure/coursescourse-idmodulesmodule-iditems-post-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/items/master/_listings/instructure/coursescourse-idmodulesmodule-iditems-post-openapi.md
- name: Instructure Canvas Courses API Delete module item
  x-api-slug: instructure-canvas-courses-api
  description: Delete module item.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/820-instructure.jpg
  humanURL: http://instructure.com
  baseURL: https://canvas.instructure.com//api/v1//courses/{course_id}/modules/module_id/items/{id}
  tags: Courses,Course,Id,Modules,Module,Id,Items,Id
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/items/master/_listings/instructure/coursescourse-idmodulesmodule-iditemsid-delete-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/items/master/_listings/instructure/coursescourse-idmodulesmodule-iditemsid-delete-openapi.md
- name: Instructure Canvas Courses API Show module item
  x-api-slug: instructure-canvas-courses-api
  description: Show module item.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/820-instructure.jpg
  humanURL: http://instructure.com
  baseURL: https://canvas.instructure.com//api/v1//courses/{course_id}/modules/module_id/items/{id}
  tags: Courses,Course,Id,Modules,Module,Id,Items,Id
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/items/master/_listings/instructure/coursescourse-idmodulesmodule-iditemsid-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/items/master/_listings/instructure/coursescourse-idmodulesmodule-iditemsid-get-openapi.md
- name: Instructure Canvas Courses API Update a module item
  x-api-slug: instructure-canvas-courses-api
  description: Update a module item.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/820-instructure.jpg
  humanURL: http://instructure.com
  baseURL: https://canvas.instructure.com//api/v1//courses/{course_id}/modules/module_id/items/{id}
  tags: Courses,Course,Id,Modules,Module,Id,Items,Id
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/items/master/_listings/instructure/coursescourse-idmodulesmodule-iditemsid-put-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/items/master/_listings/instructure/coursescourse-idmodulesmodule-iditemsid-put-openapi.md
- name: Instructure Canvas Courses API Mark module item as done/not done
  x-api-slug: instructure-canvas-courses-api
  description: Mark module item as done/not done.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/820-instructure.jpg
  humanURL: http://instructure.com
  baseURL: https://canvas.instructure.com//api/v1//courses/{course_id}/modules/module_id/items/{id}/done
  tags: Courses,Course,Id,Modules,Module,Id,Items,Id,Done
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/items/master/_listings/instructure/coursescourse-idmodulesmodule-iditemsiddone-put-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/items/master/_listings/instructure/coursescourse-idmodulesmodule-iditemsiddone-put-openapi.md
- name: Instructure Canvas Courses API Mark module item read
  x-api-slug: instructure-canvas-courses-api
  description: Mark module item read.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/820-instructure.jpg
  humanURL: http://instructure.com
  baseURL: https://canvas.instructure.com//api/v1//courses/{course_id}/modules/module_id/items/{id}/mark_read
  tags: Courses,Course,Id,Modules,Module,Id,Items,Id,Mark,Read
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/items/master/_listings/instructure/coursescourse-idmodulesmodule-iditemsidmark-read-post-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/items/master/_listings/instructure/coursescourse-idmodulesmodule-iditemsidmark-read-post-openapi.md
- name: Instructure Canvas Courses API
  x-api-slug: instructure-canvas-courses-api
  description: Instructure makes software that makes smarter people. Products include
    Canvas LMS, Bridge and Canvas Network.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/820-instructure.jpg
  humanURL: http://instructure.com
  baseURL: https://canvas.instructure.com//api/v1
  tags: Items
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/items/master/_listings/instructure/openapi.md
x-common:
- type: x-blog
  url: http://blog.instructure.com
- type: x-blog-rss
  url: http://voice.instructure.com/CMS/UI/Modules/BizBlogger/rss.aspx?tabid=772438&moduleid=1638884&maxcount=25&t=415c2e5d197a4d6f7cdcc81385b677f1
- type: x-crunchbase
  url: https://crunchbase.com/organization/instructure
- type: x-crunchbase
  url: http://www.crunchbase.com/company/instructure
- type: x-email
  url: info@instructure.com
- type: x-email
  url: jobs@instructure.com
- type: x-email
  url: privacy@instructure.com
- type: x-email
  url: legal@instructure.com
- type: x-github
  url: https://github.com/instructure
- type: x-twitter
  url: https://twitter.com/instructure
- type: x-website
  url: http://instructure.com
- type: x-website
  url: https://canvas.instructure.com/doc/api/index.html
include: []
maintainers:
- FN: Kin Lane
  x-twitter: apievangelist
  email: info@apievangelist.com
---