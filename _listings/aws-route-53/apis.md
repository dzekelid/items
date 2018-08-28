---
name: AWS Route 53
x-slug: aws-route-53
description: Amazon Route 53 is a highly available and scalable cloud Domain Name
  System (DNS) web service. It is designed to give developers and businesses an extremely
  reliable and cost effective way to route end users to Internet applications by translating
  names like www.example.com into the numeric IP addresses like 192.0.2.1 that computers
  use to connect to each other. Amazon Route 53 is fully compliant with IPv6 as well.Amazon
  Route 53 effectively connects user requests to infrastructure running in AWS &ndash;
  such as Amazon EC2 instances, Elastic Load Balancing load balancers, or Amazon S3
  buckets &ndash; and can also be used to route users to infrastructure outside of
  AWS. You can use Amazon Route 53 to configure DNS health checks to route traffic
  to healthy endpoints or to independently monitor the health of your application
  and its endpoints. Amazon Route 53 Traffic Flow makes it easy for you to manage
  traffic globally through a variety of routing types, including Latency Based Routing,
  Geo DNS, and Weighted Round Robin&mdash;all of which can be combined with DNS Failover
  in order to enable a variety of low-latency, fault-tolerant architectures. Using
  Amazon Route 53 Traffic Flow&rsquo;s simple visual editor, you can easily manage
  how your end-users are routed to your application&rsquo;s endpoints&mdash;whether
  in a single AWS region or distributed around the globe. Amazon Route 53 also offers
  Domain Name Registration &ndash; you can purchase and manage domain names such as
  example.com and Amazon Route 53 will automatically configure DNS settings for your
  domains.
image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/Networking_AmazonRoute53.png
x-kinRank: "8"
x-alexaRank: "0"
tags: Items
created: "2018-08-27"
modified: "2018-08-27"
url: https://raw.githubusercontent.com/streamdata-gallery-topics/items/master/_listings/aws-route-53/apis.md
specificationVersion: "0.14"
apis:
- name: AWS Route 53 API - List Reusable Delegation Sets
  x-api-slug: 20130401delegationsetmarkermarkerampmaxitemsmaxitems-get
  description: To retrieve a list of your reusable delegation sets, send a GET request
    tothe /2013-04-01/delegationset resource. The response to this request includes
    aDelegationSets element with zero, one, or multiple DelegationSetchild elements.
    By default, the list of delegation sets is displayed on a single page. You cancontrol
    the length of the page that is displayed by using the MaxItems parameter.You can
    use the Marker parameter to control the delegation set that the listbegins with.
    Note Amazon Route 53 returns a maximum of 100 items. If you set MaxItems to a
    value greater than100, Amazon Route 53 returns only the first 100.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/Networking_AmazonRoute53.png
  humanURL: https://aws.amazon.com/route53/
  baseURL: :///
  tags: Amazon Web Services, DNS, API Service Provider, API Service Provider, API
    Provider, Profiles, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/items/master/_listings/aws-route-53/20130401delegationsetmarkermarkerampmaxitemsmaxitems-get-openapi.md
- name: AWS Route 53 API - List Geo Locations
  x-api-slug: 20130401geolocationsampmaxitemsmaxitemsstartcontinentcodestartcontinentcodeampstartcountrycodestartcountrycodeampstartsubdivisioncodestartsubdivisioncode-get
  description: Retrieves a list of supported geo locations. Send a GET request to
    the/2013-04-01/geolocations resource. The response to this request includes aGeoLocationDetailsList
    element for each location that Amazon Route 53 supports.Countries are listed first,
    and continents are listed last. If Amazon Route 53 supportssubdivisions for a
    country (for example, states or provinces), the subdivisions for thatcountry are
    listed in alphabetical order immediately after the corresponding country.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/Networking_AmazonRoute53.png
  humanURL: https://aws.amazon.com/route53/
  baseURL: :///
  tags: Amazon Web Services, DNS, API Service Provider, API Service Provider, API
    Provider, Profiles, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/items/master/_listings/aws-route-53/20130401geolocationsampmaxitemsmaxitemsstartcontinentcodestartcontinentcodeampstartcountrycodestartcountrycodeampstartsubdivisioncodestartsubdivisioncode-get-openapi.md
- name: AWS Route 53 API - List Health Checks
  x-api-slug: 20130401healthcheckmarkermarkerampmaxitemsmaxitems-get
  description: Retrieve a list of your health checks. Send a GET request to the/2013-04-01/healthcheck
    resource. The response to this request includes aHealthChecks element with zero
    or more HealthCheck child elements.By default, the list of health checks is displayed
    on a single page. You can control thelength of the page that is displayed by using
    the MaxItems parameter. You can usethe Marker parameter to control the health
    check that the list beginswith.For information about listing health checks using
    the Amazon Route 53 console, see Amazon Route 53 Health Checks and DNS Failover.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/Networking_AmazonRoute53.png
  humanURL: https://aws.amazon.com/route53/
  baseURL: :///
  tags: Amazon Web Services, DNS, API Service Provider, API Service Provider, API
    Provider, Profiles, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/items/master/_listings/aws-route-53/20130401healthcheckmarkermarkerampmaxitemsmaxitems-get-openapi.md
- name: AWS Route 53 API - List Hosted Zones
  x-api-slug: 20130401hostedzoneampdelegationsetiddelegationsetidmarkermarkerampmaxitemsmaxitems-get
  description: 'To retrieve a list of your public and private hosted zones, send a
    GETrequest to the /2013-04-01/hostedzone resource. The response to this requestincludes
    a HostedZones child element for each hosted zone created by the currentAWS account.Amazon
    Route 53 returns a maximum of 100 items in each response. If you have a lot of
    hostedzones, you can use the maxitems parameter to list them in groups of up to
    100.The response includes four values that help navigate from one group of maxitemshosted
    zones to the next:                  MaxItems is the value specified for the maxitems
    parameterin the request that produced the current response.If the value of IsTruncated
    in the response is true, there are morehosted zones associated with the current
    AWS account.                   NextMarker is the hosted zone ID of the next hosted
    zone that isassociated with the current AWS account. If you want to list more
    hosted zones, makeanother call to ListHostedZones, and specify the value of theNextMarker
    element in the marker parameter. If IsTruncated is false, the NextMarker element
    isomitted from the response.If you''re making the second or subsequent call to
    ListHostedZones, theMarker element matches the value that you specified in themarker
    parameter in the previous request.'
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/Networking_AmazonRoute53.png
  humanURL: https://aws.amazon.com/route53/
  baseURL: :///
  tags: Amazon Web Services, DNS, API Service Provider, API Service Provider, API
    Provider, Profiles, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/items/master/_listings/aws-route-53/20130401hostedzoneampdelegationsetiddelegationsetidmarkermarkerampmaxitemsmaxitems-get-openapi.md
- name: AWS Route 53 API - List V P C Association Authorizations
  x-api-slug: 20130401hostedzoneidauthorizevpcassociationampmaxresultsmaxresultsnexttokennexttoken-get
  description: 'Gets a list of the VPCs that were created by other accounts and that
    can be associated with a specified hosted zone because you''ve submitted one or
    more CreateVPCAssociationAuthorization requests. Send a GET request to the /2013-04-01/hostedzone/hosted
    zone ID/authorizevpcassociation resource. The response to this request includes
    a VPCs element with a VPC child element for each VPC that can be associated with
    the hosted zone.Amazon Route 53 returns up to 50 VPCs per page. To return fewer
    VPCs per page, include the MaxResults parameter:             /2013-04-01/hostedzone/hosted
    zone ID/authorizevpcassociation?MaxItems=VPCs per page                     If
    the response includes a NextToken element, there are more VPCs to list. To get
    the next page of VPCs, submit another ListVPCAssociationAuthorizations request,
    and include the value of the NextToken element from the response in the NextToken
    request parameter:            /2013-04-01/hostedzone/hosted zone ID/authorizevpcassociation?MaxItems=VPCs
    per page&amp;NextToken='
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/Networking_AmazonRoute53.png
  humanURL: https://aws.amazon.com/route53/
  baseURL: :///
  tags: Amazon Web Services, DNS, API Service Provider, API Service Provider, API
    Provider, Profiles, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/items/master/_listings/aws-route-53/20130401hostedzoneidauthorizevpcassociationampmaxresultsmaxresultsnexttokennexttoken-get-openapi.md
- name: AWS Route 53 API - List Resource Record Sets
  x-api-slug: 20130401hostedzoneidrrsetampidentifierstartrecordidentifierampmaxitemsmaxitemsnamestartrecordnameamptypestartrecordtype-get
  description: 'Lists the resource record sets in a specified hosted zone.            ListResourceRecordSets
    returns up to 100 resource record sets at a time in ASCII order, beginning at
    a position specified by the name and type elements. The action sorts results first
    by DNS name with the labels reversed, for example:            com.example.www.         Note
    the trailing dot, which can change the sort order in some circumstances.When multiple
    records have the same DNS name, the action sorts results by the record type.You
    can use the name and type elements to adjust the beginning position of the list
    of resource record sets returned:If you do not specify Name or TypeThe results
    begin with the first resource record set that the hosted zone contains.If you
    specify Name but not TypeThe results begin with the first resource record set
    in the list whose name is greater than or equal to Name.If you specify Type but
    not NameAmazon Route 53 returns the InvalidInput error.If you specify both Name
    and TypeThe results begin with the first resource record set in the list whose
    name is greater than or equal to Name, and whose type is greater than or equal
    to Type.This action returns the most current version of the records. This includes
    records that are PENDING, and that are not yet available on all Amazon Route 53
    DNS servers.To ensure that you get an accurate listing of the resource record
    sets for a hosted zone at a point in time, do not submit a ChangeResourceRecordSets
    request while you''re paging through the results of a ListResourceRecordSets request.
    If you do, some pages may display results without the latest changes while other
    pages display results with the latest changes.'
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/Networking_AmazonRoute53.png
  humanURL: https://aws.amazon.com/route53/
  baseURL: :///
  tags: Amazon Web Services, DNS, API Service Provider, API Service Provider, API
    Provider, Profiles, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/items/master/_listings/aws-route-53/20130401hostedzoneidrrsetampidentifierstartrecordidentifierampmaxitemsmaxitemsnamestartrecordnameamptypestartrecordtype-get-openapi.md
- name: AWS Route 53 API - List Hosted Zones By Name
  x-api-slug: 20130401hostedzonesbynamednsnamednsnameamphostedzoneidhostedzoneidampmaxitemsmaxitems-get
  description: 'Retrieves a list of your hosted zones in lexicographic order. Send
    a GETrequest to the /2013-04-01/hostedzonesbyname resource. The response includes
    aHostedZones child element for each hosted zone created by the current AWSaccount.             ListHostedZonesByName
    sorts hosted zones by name with the labels reversed.For example:                  com.example.www.               Note
    the trailing dot, which can change the sort order in some circumstances.If the
    domain name includes escape characters or Punycode,ListHostedZonesByName alphabetizes
    the domain name using the escaped orPunycoded value, which is the format that
    Amazon Route 53 saves in its database. For example, to createa hosted zone for
    example.com, specify ex\344mple.com for the domain name.ListHostedZonesByName
    alphabetizes it as:                  com.ex\344mple.               The labels
    are reversed and alphabetized using the escaped value. For more informationabout
    valid domain name formats, including internationalized domain names, see DNS Domain
    Name Format in theAmazon Route 53 Developer Guide.Amazon Route 53 returns up to
    100 items in each response. If you have a lot of hosted zones, usethe MaxItems
    parameter to list them in groups of up to 100. The response includesvalues that
    help navigate from one group of MaxItems hosted zones to thenext:The DNSName and
    HostedZoneId elements in the responsecontain the values, if any, specified for
    the dnsname andhostedzoneid parameters in the request that produced the currentresponse.The
    MaxItems element in the response contains the value, if any, thatyou specified
    for the maxitems parameter in the request that produced thecurrent response.If
    the value of IsTruncated in the response is true, there are morehosted zones associated
    with the current AWS account. If IsTruncated is false, this response includes
    the last hosted zonethat is associated with the current account. The NextDNSName
    element andNextHostedZoneId elements are omitted from the response.The NextDNSName
    and NextHostedZoneId elements in theresponse contain the domain name and the hosted
    zone ID of the next hosted zone that isassociated with the current AWS account.
    If you want to list more hosted zones, makeanother call to ListHostedZonesByName,
    and specify the value ofNextDNSName and NextHostedZoneId in the dnsnameand hostedzoneid
    parameters, respectively.'
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/Networking_AmazonRoute53.png
  humanURL: https://aws.amazon.com/route53/
  baseURL: :///
  tags: Amazon Web Services, DNS, API Service Provider, API Service Provider, API
    Provider, Profiles, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/items/master/_listings/aws-route-53/20130401hostedzonesbynamednsnamednsnameamphostedzoneidhostedzoneidampmaxitemsmaxitems-get-openapi.md
- name: AWS Route 53 API - List Traffic Policies
  x-api-slug: 20130401trafficpoliciesampmaxitemsmaxitemstrafficpolicyidtrafficpolicyidmarker-get
  description: 'Gets information about the latest version for every traffic policy
    that is associatedwith the current AWS account. Send a GET request to the /Amazon
    Route 53API version/trafficpolicy resource.Amazon Route 53 returns a maximum of
    100 items in each response. If you have a lot of trafficpolicies, you can use
    the maxitems parameter to list them in groups of up to100.The response includes
    three values that help you navigate from one group ofmaxitems traffic policies
    to the next:             IsTruncated           If the value of IsTruncated in
    the response is true,there are more traffic policies associated with the current
    AWS account.If IsTruncated is false, this response includes the lasttraffic policy
    that is associated with the current account.             TrafficPolicyIdMarker           If
    IsTruncated is true,TrafficPolicyIdMarker is the ID of the first traffic policy
    in the nextgroup of MaxItems traffic policies. If you want to list more trafficpolicies,
    make another call to ListTrafficPolicies, and specify the value ofthe TrafficPolicyIdMarker
    element from the response in theTrafficPolicyIdMarker request parameter.If IsTruncated
    is false, theTrafficPolicyIdMarker element is omitted from the response.             MaxItems           The
    value that you specified for the MaxItems parameter in the requestthat produced
    the current response.'
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/Networking_AmazonRoute53.png
  humanURL: https://aws.amazon.com/route53/
  baseURL: :///
  tags: Amazon Web Services, DNS, API Service Provider, API Service Provider, API
    Provider, Profiles, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/items/master/_listings/aws-route-53/20130401trafficpoliciesampmaxitemsmaxitemstrafficpolicyidtrafficpolicyidmarker-get-openapi.md
- name: AWS Route 53 API - List Traffic Policy Versions
  x-api-slug: 20130401trafficpoliciesidversionsampmaxitemsmaxitemstrafficpolicyversiontrafficpolicyversionmarker-get
  description: 'Gets information about all of the versions for a specified traffic
    policy.Send a GET request to the /Amazon Route 53 APIversion/trafficpolicy resource
    and specify the ID of the traffic policyfor which you want to list versions.Amazon
    Route 53 returns a maximum of 100 items in each response. If you have a lot of
    trafficpolicies, you can use the maxitems parameter to list them in groups of
    up to100.The response includes three values that help you navigate from one group
    ofmaxitems traffic policies to the next:             IsTruncated           If
    the value of IsTruncated in the response is true,there are more traffic policy
    versions associated with the specified trafficpolicy.If IsTruncated is false,
    this response includes the lasttraffic policy version that is associated with
    the specified traffic policy.             TrafficPolicyVersionMarker           The
    ID of the next traffic policy version that is associated with the current AWSaccount.
    If you want to list more traffic policies, make another call toListTrafficPolicyVersions,
    and specify the value of theTrafficPolicyVersionMarker element in theTrafficPolicyVersionMarker
    request parameter.If IsTruncated is false, Amazon Route 53 omits theTrafficPolicyVersionMarker
    element from the response.             MaxItems           The value that you specified
    for the MaxItems parameter in the requestthat produced the current response.'
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/Networking_AmazonRoute53.png
  humanURL: https://aws.amazon.com/route53/
  baseURL: :///
  tags: Amazon Web Services, DNS, API Service Provider, API Service Provider, API
    Provider, Profiles, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/items/master/_listings/aws-route-53/20130401trafficpoliciesidversionsampmaxitemsmaxitemstrafficpolicyversiontrafficpolicyversionmarker-get-openapi.md
- name: AWS Route 53 API - List Traffic Policy Instances By Hosted Zone
  x-api-slug: 20130401trafficpolicyinstanceshostedzoneidhostedzoneidampmaxitemsmaxitemsamptrafficpolicyinstancenametrafficpolicyinstancenamemarkeramptrafficpolicyinstancetypetrafficpolicyinstancetypemarker-get
  description: 'Gets information about the traffic policy instances that you created
    in a specifiedhosted zone.NoteAfter you submit an UpdateTrafficPolicyInstance
    request, there''s a briefdelay while Amazon Route 53 creates the resource record
    sets that are specified in the traffic policydefinition. For more information,
    see the State response element.Send a GET request to the /Amazon Route 53 APIversion/trafficpolicyinstance
    resource and include the ID of the hostedzone.Amazon Route 53 returns a maximum
    of 100 items in each response. If you have a lot of trafficpolicy instances, you
    can use the MaxItems parameter to list them in groups of upto 100.The response
    includes four values that help you navigate from one group ofMaxItems traffic
    policy instances to the next:             IsTruncated               If the value
    of IsTruncated in the response is true, there aremore traffic policy instances
    associated with the current AWS account.If IsTruncated is false, this response
    includes the lasttraffic policy instance that is associated with the current account.             MaxItems           The
    value that you specified for the MaxItems parameter in the requestthat produced
    the current response.                  TrafficPolicyInstanceNameMarker and TrafficPolicyInstanceTypeMarker               If
    IsTruncated is true, these two values in the responserepresent the first traffic
    policy instance in the next group of MaxItemstraffic policy instances. To list
    more traffic policy instances, make another call toListTrafficPolicyInstancesByHostedZone,
    and specify these values in thecorresponding request parameters.If IsTruncated
    is false, all three elements are omittedfrom the response.'
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/Networking_AmazonRoute53.png
  humanURL: https://aws.amazon.com/route53/
  baseURL: :///
  tags: Amazon Web Services, DNS, API Service Provider, API Service Provider, API
    Provider, Profiles, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/items/master/_listings/aws-route-53/20130401trafficpolicyinstanceshostedzoneidhostedzoneidampmaxitemsmaxitemsamptrafficpolicyinstancenametrafficpolicyinstancenamemarkeramptrafficpolicyinstancetypetrafficpolicyinstancetypemarker-get-openapi.md
- name: AWS Route 53 API - List Traffic Policy Instances By Policy
  x-api-slug: 20130401trafficpolicyinstancestrafficpolicyamphostedzoneidhostedzoneidmarkeridtrafficpolicyidampmaxitemsmaxitemsamptrafficpolicyinstancenametrafficpolicyinstancenamemarkeramptrafficpolicyinstancetypetrafficpolicyinstancetypemarker-get
  description: 'Gets information about the traffic policy instances that you created
    by using a specifytraffic policy version.NoteAfter you submit a CreateTrafficPolicyInstance
    or anUpdateTrafficPolicyInstance request, there''s a brief delay while Amazon
    Route 53creates the resource record sets that are specified in the traffic policy
    definition. Formore information, see the State response element.Send a GET request
    to the /Route 53 APIversion/trafficpolicyinstance resource and include the ID
    and version ofthe traffic policy.Amazon Route 53 returns a maximum of 100 items
    in each response. If you have a lot of trafficpolicy instances, you can use the
    MaxItems parameter to list them in groups of upto 100.The response includes five
    values that help you navigate from one group ofMaxItems traffic policy instances
    to the next:             IsTruncated               If the value of IsTruncated
    in the response is true,there are more traffic policy instances associated with
    the specified trafficpolicy.If IsTruncated is false, this response includes the
    lasttraffic policy instance that is associated with the specified traffic policy.             MaxItems               The
    value that you specified for the MaxItems parameter in the requestthat produced
    the current response.                  HostedZoneIdMarker, TrafficPolicyInstanceNameMarker,
    and TrafficPolicyInstanceTypeMarker               If IsTruncated is true, these
    values in the responserepresent the first traffic policy instance in the next
    group of MaxItemstraffic policy instances. To list more traffic policy instances,
    make another call toListTrafficPolicyInstancesByPolicy, and specify these values
    in thecorresponding request parameters.If IsTruncated is false, all three elements
    are omittedfrom the response.'
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/Networking_AmazonRoute53.png
  humanURL: https://aws.amazon.com/route53/
  baseURL: :///
  tags: Amazon Web Services, DNS, API Service Provider, API Service Provider, API
    Provider, Profiles, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/items/master/_listings/aws-route-53/20130401trafficpolicyinstancestrafficpolicyamphostedzoneidhostedzoneidmarkeridtrafficpolicyidampmaxitemsmaxitemsamptrafficpolicyinstancenametrafficpolicyinstancenamemarkeramptrafficpolicyinstancetypetrafficpolicyinstancetypemarker-get-openapi.md
- name: AWS Route 53 API - List Traffic Policy Instances
  x-api-slug: 20130401trafficpolicyinstanceshostedzoneidhostedzoneidmarkerampmaxitemsmaxitemsamptrafficpolicyinstancenametrafficpolicyinstancenamemarkeramptrafficpolicyinstancetypetrafficpolicyinstancetypemarker-get
  description: 'Gets information about the traffic policy instances that you created
    by using thecurrent AWS account.NoteAfter you submit an UpdateTrafficPolicyInstance
    request, there''s a briefdelay while Amazon Route 53 creates the resource record
    sets that are specified in the traffic policydefinition. For more information,
    see the State response element.Send a GET request to the /Amazon Route 53 APIversion/trafficpolicyinstance
    resource.Amazon Route 53 returns a maximum of 100 items in each response. If you
    have a lot of trafficpolicy instances, you can use the MaxItems parameter to list
    them in groups of upto 100.The response includes five values that help you navigate
    from one group ofMaxItems traffic policy instances to the next:             IsTruncated           If
    the value of IsTruncated in the response is true,there are more traffic policy
    instances associated with the current AWSaccount.If IsTruncated is false, this
    response includes the lasttraffic policy instance that is associated with the
    current account.             MaxItems           The value that you specified for
    the MaxItems parameter in the requestthat produced the current response.                  HostedZoneIdMarker,
    TrafficPolicyInstanceNameMarker, and TrafficPolicyInstanceTypeMarker               If
    IsTruncated is true, these three values in theresponse represent the first traffic
    policy instance in the next group ofMaxItems traffic policy instances. To list
    more traffic policy instances,make another call to ListTrafficPolicyInstances,
    and specify these values inthe corresponding request parameters.If IsTruncated
    is false, all three elements are omittedfrom the response.'
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/Networking_AmazonRoute53.png
  humanURL: https://aws.amazon.com/route53/
  baseURL: :///
  tags: Amazon Web Services, DNS, API Service Provider, API Service Provider, API
    Provider, Profiles, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/items/master/_listings/aws-route-53/20130401trafficpolicyinstanceshostedzoneidhostedzoneidmarkerampmaxitemsmaxitemsamptrafficpolicyinstancenametrafficpolicyinstancenamemarkeramptrafficpolicyinstancetypetrafficpolicyinstancetypemarker-get-openapi.md
- name: AWS Route 53 API - List Reusable Delegation Sets
  x-api-slug: 20130401delegationsetmarkermarkerampmaxitemsmaxitems-get
  description: To retrieve a list of your reusable delegation sets, send a GET request
    tothe /2013-04-01/delegationset resource. The response to this request includes
    aDelegationSets element with zero, one, or multiple DelegationSetchild elements.
    By default, the list of delegation sets is displayed on a single page. You cancontrol
    the length of the page that is displayed by using the MaxItems parameter.You can
    use the Marker parameter to control the delegation set that the listbegins with.
    Note Amazon Route 53 returns a maximum of 100 items. If you set MaxItems to a
    value greater than100, Amazon Route 53 returns only the first 100.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/Networking_AmazonRoute53.png
  humanURL: https://aws.amazon.com/route53/
  baseURL: :///
  tags: Amazon Web Services, DNS, API Service Provider, API Service Provider, API
    Provider, Profiles, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/items/master/_listings/aws-route-53/20130401delegationsetmarkermarkerampmaxitemsmaxitems-get-openapi.md
- name: AWS Route 53 API - List Geo Locations
  x-api-slug: 20130401geolocationsampmaxitemsmaxitemsstartcontinentcodestartcontinentcodeampstartcountrycodestartcountrycodeampstartsubdivisioncodestartsubdivisioncode-get
  description: Retrieves a list of supported geo locations. Send a GET request to
    the/2013-04-01/geolocations resource. The response to this request includes aGeoLocationDetailsList
    element for each location that Amazon Route 53 supports.Countries are listed first,
    and continents are listed last. If Amazon Route 53 supportssubdivisions for a
    country (for example, states or provinces), the subdivisions for thatcountry are
    listed in alphabetical order immediately after the corresponding country.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/Networking_AmazonRoute53.png
  humanURL: https://aws.amazon.com/route53/
  baseURL: :///
  tags: Amazon Web Services, DNS, API Service Provider, API Service Provider, API
    Provider, Profiles, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/items/master/_listings/aws-route-53/20130401geolocationsampmaxitemsmaxitemsstartcontinentcodestartcontinentcodeampstartcountrycodestartcountrycodeampstartsubdivisioncodestartsubdivisioncode-get-openapi.md
- name: AWS Route 53 API - List Health Checks
  x-api-slug: 20130401healthcheckmarkermarkerampmaxitemsmaxitems-get
  description: Retrieve a list of your health checks. Send a GET request to the/2013-04-01/healthcheck
    resource. The response to this request includes aHealthChecks element with zero
    or more HealthCheck child elements.By default, the list of health checks is displayed
    on a single page. You can control thelength of the page that is displayed by using
    the MaxItems parameter. You can usethe Marker parameter to control the health
    check that the list beginswith.For information about listing health checks using
    the Amazon Route 53 console, see Amazon Route 53 Health Checks and DNS Failover.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/Networking_AmazonRoute53.png
  humanURL: https://aws.amazon.com/route53/
  baseURL: :///
  tags: Amazon Web Services, DNS, API Service Provider, API Service Provider, API
    Provider, Profiles, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/items/master/_listings/aws-route-53/20130401healthcheckmarkermarkerampmaxitemsmaxitems-get-openapi.md
- name: AWS Route 53 API - List Hosted Zones
  x-api-slug: 20130401hostedzoneampdelegationsetiddelegationsetidmarkermarkerampmaxitemsmaxitems-get
  description: 'To retrieve a list of your public and private hosted zones, send a
    GETrequest to the /2013-04-01/hostedzone resource. The response to this requestincludes
    a HostedZones child element for each hosted zone created by the currentAWS account.Amazon
    Route 53 returns a maximum of 100 items in each response. If you have a lot of
    hostedzones, you can use the maxitems parameter to list them in groups of up to
    100.The response includes four values that help navigate from one group of maxitemshosted
    zones to the next:                  MaxItems is the value specified for the maxitems
    parameterin the request that produced the current response.If the value of IsTruncated
    in the response is true, there are morehosted zones associated with the current
    AWS account.                   NextMarker is the hosted zone ID of the next hosted
    zone that isassociated with the current AWS account. If you want to list more
    hosted zones, makeanother call to ListHostedZones, and specify the value of theNextMarker
    element in the marker parameter. If IsTruncated is false, the NextMarker element
    isomitted from the response.If you''re making the second or subsequent call to
    ListHostedZones, theMarker element matches the value that you specified in themarker
    parameter in the previous request.'
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/Networking_AmazonRoute53.png
  humanURL: https://aws.amazon.com/route53/
  baseURL: :///
  tags: Amazon Web Services, DNS, API Service Provider, API Service Provider, API
    Provider, Profiles, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/items/master/_listings/aws-route-53/20130401hostedzoneampdelegationsetiddelegationsetidmarkermarkerampmaxitemsmaxitems-get-openapi.md
- name: AWS Route 53 API - List V P C Association Authorizations
  x-api-slug: 20130401hostedzoneidauthorizevpcassociationampmaxresultsmaxresultsnexttokennexttoken-get
  description: 'Gets a list of the VPCs that were created by other accounts and that
    can be associated with a specified hosted zone because you''ve submitted one or
    more CreateVPCAssociationAuthorization requests. Send a GET request to the /2013-04-01/hostedzone/hosted
    zone ID/authorizevpcassociation resource. The response to this request includes
    a VPCs element with a VPC child element for each VPC that can be associated with
    the hosted zone.Amazon Route 53 returns up to 50 VPCs per page. To return fewer
    VPCs per page, include the MaxResults parameter:             /2013-04-01/hostedzone/hosted
    zone ID/authorizevpcassociation?MaxItems=VPCs per page                     If
    the response includes a NextToken element, there are more VPCs to list. To get
    the next page of VPCs, submit another ListVPCAssociationAuthorizations request,
    and include the value of the NextToken element from the response in the NextToken
    request parameter:            /2013-04-01/hostedzone/hosted zone ID/authorizevpcassociation?MaxItems=VPCs
    per page&amp;NextToken='
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/Networking_AmazonRoute53.png
  humanURL: https://aws.amazon.com/route53/
  baseURL: :///
  tags: Amazon Web Services, DNS, API Service Provider, API Service Provider, API
    Provider, Profiles, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/items/master/_listings/aws-route-53/20130401hostedzoneidauthorizevpcassociationampmaxresultsmaxresultsnexttokennexttoken-get-openapi.md
- name: AWS Route 53 API - List Resource Record Sets
  x-api-slug: 20130401hostedzoneidrrsetampidentifierstartrecordidentifierampmaxitemsmaxitemsnamestartrecordnameamptypestartrecordtype-get
  description: 'Lists the resource record sets in a specified hosted zone.            ListResourceRecordSets
    returns up to 100 resource record sets at a time in ASCII order, beginning at
    a position specified by the name and type elements. The action sorts results first
    by DNS name with the labels reversed, for example:            com.example.www.         Note
    the trailing dot, which can change the sort order in some circumstances.When multiple
    records have the same DNS name, the action sorts results by the record type.You
    can use the name and type elements to adjust the beginning position of the list
    of resource record sets returned:If you do not specify Name or TypeThe results
    begin with the first resource record set that the hosted zone contains.If you
    specify Name but not TypeThe results begin with the first resource record set
    in the list whose name is greater than or equal to Name.If you specify Type but
    not NameAmazon Route 53 returns the InvalidInput error.If you specify both Name
    and TypeThe results begin with the first resource record set in the list whose
    name is greater than or equal to Name, and whose type is greater than or equal
    to Type.This action returns the most current version of the records. This includes
    records that are PENDING, and that are not yet available on all Amazon Route 53
    DNS servers.To ensure that you get an accurate listing of the resource record
    sets for a hosted zone at a point in time, do not submit a ChangeResourceRecordSets
    request while you''re paging through the results of a ListResourceRecordSets request.
    If you do, some pages may display results without the latest changes while other
    pages display results with the latest changes.'
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/Networking_AmazonRoute53.png
  humanURL: https://aws.amazon.com/route53/
  baseURL: :///
  tags: Amazon Web Services, DNS, API Service Provider, API Service Provider, API
    Provider, Profiles, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/items/master/_listings/aws-route-53/20130401hostedzoneidrrsetampidentifierstartrecordidentifierampmaxitemsmaxitemsnamestartrecordnameamptypestartrecordtype-get-openapi.md
- name: AWS Route 53 API - List Hosted Zones By Name
  x-api-slug: 20130401hostedzonesbynamednsnamednsnameamphostedzoneidhostedzoneidampmaxitemsmaxitems-get
  description: 'Retrieves a list of your hosted zones in lexicographic order. Send
    a GETrequest to the /2013-04-01/hostedzonesbyname resource. The response includes
    aHostedZones child element for each hosted zone created by the current AWSaccount.             ListHostedZonesByName
    sorts hosted zones by name with the labels reversed.For example:                  com.example.www.               Note
    the trailing dot, which can change the sort order in some circumstances.If the
    domain name includes escape characters or Punycode,ListHostedZonesByName alphabetizes
    the domain name using the escaped orPunycoded value, which is the format that
    Amazon Route 53 saves in its database. For example, to createa hosted zone for
    example.com, specify ex\344mple.com for the domain name.ListHostedZonesByName
    alphabetizes it as:                  com.ex\344mple.               The labels
    are reversed and alphabetized using the escaped value. For more informationabout
    valid domain name formats, including internationalized domain names, see DNS Domain
    Name Format in theAmazon Route 53 Developer Guide.Amazon Route 53 returns up to
    100 items in each response. If you have a lot of hosted zones, usethe MaxItems
    parameter to list them in groups of up to 100. The response includesvalues that
    help navigate from one group of MaxItems hosted zones to thenext:The DNSName and
    HostedZoneId elements in the responsecontain the values, if any, specified for
    the dnsname andhostedzoneid parameters in the request that produced the currentresponse.The
    MaxItems element in the response contains the value, if any, thatyou specified
    for the maxitems parameter in the request that produced thecurrent response.If
    the value of IsTruncated in the response is true, there are morehosted zones associated
    with the current AWS account. If IsTruncated is false, this response includes
    the last hosted zonethat is associated with the current account. The NextDNSName
    element andNextHostedZoneId elements are omitted from the response.The NextDNSName
    and NextHostedZoneId elements in theresponse contain the domain name and the hosted
    zone ID of the next hosted zone that isassociated with the current AWS account.
    If you want to list more hosted zones, makeanother call to ListHostedZonesByName,
    and specify the value ofNextDNSName and NextHostedZoneId in the dnsnameand hostedzoneid
    parameters, respectively.'
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/Networking_AmazonRoute53.png
  humanURL: https://aws.amazon.com/route53/
  baseURL: :///
  tags: Amazon Web Services, DNS, API Service Provider, API Service Provider, API
    Provider, Profiles, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/items/master/_listings/aws-route-53/20130401hostedzonesbynamednsnamednsnameamphostedzoneidhostedzoneidampmaxitemsmaxitems-get-openapi.md
- name: AWS Route 53 API - List Traffic Policies
  x-api-slug: 20130401trafficpoliciesampmaxitemsmaxitemstrafficpolicyidtrafficpolicyidmarker-get
  description: 'Gets information about the latest version for every traffic policy
    that is associatedwith the current AWS account. Send a GET request to the /Amazon
    Route 53API version/trafficpolicy resource.Amazon Route 53 returns a maximum of
    100 items in each response. If you have a lot of trafficpolicies, you can use
    the maxitems parameter to list them in groups of up to100.The response includes
    three values that help you navigate from one group ofmaxitems traffic policies
    to the next:             IsTruncated           If the value of IsTruncated in
    the response is true,there are more traffic policies associated with the current
    AWS account.If IsTruncated is false, this response includes the lasttraffic policy
    that is associated with the current account.             TrafficPolicyIdMarker           If
    IsTruncated is true,TrafficPolicyIdMarker is the ID of the first traffic policy
    in the nextgroup of MaxItems traffic policies. If you want to list more trafficpolicies,
    make another call to ListTrafficPolicies, and specify the value ofthe TrafficPolicyIdMarker
    element from the response in theTrafficPolicyIdMarker request parameter.If IsTruncated
    is false, theTrafficPolicyIdMarker element is omitted from the response.             MaxItems           The
    value that you specified for the MaxItems parameter in the requestthat produced
    the current response.'
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/Networking_AmazonRoute53.png
  humanURL: https://aws.amazon.com/route53/
  baseURL: :///
  tags: Amazon Web Services, DNS, API Service Provider, API Service Provider, API
    Provider, Profiles, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/items/master/_listings/aws-route-53/20130401trafficpoliciesampmaxitemsmaxitemstrafficpolicyidtrafficpolicyidmarker-get-openapi.md
- name: AWS Route 53 API - List Traffic Policy Versions
  x-api-slug: 20130401trafficpoliciesidversionsampmaxitemsmaxitemstrafficpolicyversiontrafficpolicyversionmarker-get
  description: 'Gets information about all of the versions for a specified traffic
    policy.Send a GET request to the /Amazon Route 53 APIversion/trafficpolicy resource
    and specify the ID of the traffic policyfor which you want to list versions.Amazon
    Route 53 returns a maximum of 100 items in each response. If you have a lot of
    trafficpolicies, you can use the maxitems parameter to list them in groups of
    up to100.The response includes three values that help you navigate from one group
    ofmaxitems traffic policies to the next:             IsTruncated           If
    the value of IsTruncated in the response is true,there are more traffic policy
    versions associated with the specified trafficpolicy.If IsTruncated is false,
    this response includes the lasttraffic policy version that is associated with
    the specified traffic policy.             TrafficPolicyVersionMarker           The
    ID of the next traffic policy version that is associated with the current AWSaccount.
    If you want to list more traffic policies, make another call toListTrafficPolicyVersions,
    and specify the value of theTrafficPolicyVersionMarker element in theTrafficPolicyVersionMarker
    request parameter.If IsTruncated is false, Amazon Route 53 omits theTrafficPolicyVersionMarker
    element from the response.             MaxItems           The value that you specified
    for the MaxItems parameter in the requestthat produced the current response.'
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/Networking_AmazonRoute53.png
  humanURL: https://aws.amazon.com/route53/
  baseURL: :///
  tags: Amazon Web Services, DNS, API Service Provider, API Service Provider, API
    Provider, Profiles, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/items/master/_listings/aws-route-53/20130401trafficpoliciesidversionsampmaxitemsmaxitemstrafficpolicyversiontrafficpolicyversionmarker-get-openapi.md
- name: AWS Route 53 API - List Traffic Policy Instances By Hosted Zone
  x-api-slug: 20130401trafficpolicyinstanceshostedzoneidhostedzoneidampmaxitemsmaxitemsamptrafficpolicyinstancenametrafficpolicyinstancenamemarkeramptrafficpolicyinstancetypetrafficpolicyinstancetypemarker-get
  description: 'Gets information about the traffic policy instances that you created
    in a specifiedhosted zone.NoteAfter you submit an UpdateTrafficPolicyInstance
    request, there''s a briefdelay while Amazon Route 53 creates the resource record
    sets that are specified in the traffic policydefinition. For more information,
    see the State response element.Send a GET request to the /Amazon Route 53 APIversion/trafficpolicyinstance
    resource and include the ID of the hostedzone.Amazon Route 53 returns a maximum
    of 100 items in each response. If you have a lot of trafficpolicy instances, you
    can use the MaxItems parameter to list them in groups of upto 100.The response
    includes four values that help you navigate from one group ofMaxItems traffic
    policy instances to the next:             IsTruncated               If the value
    of IsTruncated in the response is true, there aremore traffic policy instances
    associated with the current AWS account.If IsTruncated is false, this response
    includes the lasttraffic policy instance that is associated with the current account.             MaxItems           The
    value that you specified for the MaxItems parameter in the requestthat produced
    the current response.                  TrafficPolicyInstanceNameMarker and TrafficPolicyInstanceTypeMarker               If
    IsTruncated is true, these two values in the responserepresent the first traffic
    policy instance in the next group of MaxItemstraffic policy instances. To list
    more traffic policy instances, make another call toListTrafficPolicyInstancesByHostedZone,
    and specify these values in thecorresponding request parameters.If IsTruncated
    is false, all three elements are omittedfrom the response.'
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/Networking_AmazonRoute53.png
  humanURL: https://aws.amazon.com/route53/
  baseURL: :///
  tags: Amazon Web Services, DNS, API Service Provider, API Service Provider, API
    Provider, Profiles, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/items/master/_listings/aws-route-53/20130401trafficpolicyinstanceshostedzoneidhostedzoneidampmaxitemsmaxitemsamptrafficpolicyinstancenametrafficpolicyinstancenamemarkeramptrafficpolicyinstancetypetrafficpolicyinstancetypemarker-get-openapi.md
- name: AWS Route 53 API - List Traffic Policy Instances By Policy
  x-api-slug: 20130401trafficpolicyinstancestrafficpolicyamphostedzoneidhostedzoneidmarkeridtrafficpolicyidampmaxitemsmaxitemsamptrafficpolicyinstancenametrafficpolicyinstancenamemarkeramptrafficpolicyinstancetypetrafficpolicyinstancetypemarker-get
  description: 'Gets information about the traffic policy instances that you created
    by using a specifytraffic policy version.NoteAfter you submit a CreateTrafficPolicyInstance
    or anUpdateTrafficPolicyInstance request, there''s a brief delay while Amazon
    Route 53creates the resource record sets that are specified in the traffic policy
    definition. Formore information, see the State response element.Send a GET request
    to the /Route 53 APIversion/trafficpolicyinstance resource and include the ID
    and version ofthe traffic policy.Amazon Route 53 returns a maximum of 100 items
    in each response. If you have a lot of trafficpolicy instances, you can use the
    MaxItems parameter to list them in groups of upto 100.The response includes five
    values that help you navigate from one group ofMaxItems traffic policy instances
    to the next:             IsTruncated               If the value of IsTruncated
    in the response is true,there are more traffic policy instances associated with
    the specified trafficpolicy.If IsTruncated is false, this response includes the
    lasttraffic policy instance that is associated with the specified traffic policy.             MaxItems               The
    value that you specified for the MaxItems parameter in the requestthat produced
    the current response.                  HostedZoneIdMarker, TrafficPolicyInstanceNameMarker,
    and TrafficPolicyInstanceTypeMarker               If IsTruncated is true, these
    values in the responserepresent the first traffic policy instance in the next
    group of MaxItemstraffic policy instances. To list more traffic policy instances,
    make another call toListTrafficPolicyInstancesByPolicy, and specify these values
    in thecorresponding request parameters.If IsTruncated is false, all three elements
    are omittedfrom the response.'
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/Networking_AmazonRoute53.png
  humanURL: https://aws.amazon.com/route53/
  baseURL: :///
  tags: Amazon Web Services, DNS, API Service Provider, API Service Provider, API
    Provider, Profiles, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/items/master/_listings/aws-route-53/20130401trafficpolicyinstancestrafficpolicyamphostedzoneidhostedzoneidmarkeridtrafficpolicyidampmaxitemsmaxitemsamptrafficpolicyinstancenametrafficpolicyinstancenamemarkeramptrafficpolicyinstancetypetrafficpolicyinstancetypemarker-get-openapi.md
- name: AWS Route 53 API - List Traffic Policy Instances
  x-api-slug: 20130401trafficpolicyinstanceshostedzoneidhostedzoneidmarkerampmaxitemsmaxitemsamptrafficpolicyinstancenametrafficpolicyinstancenamemarkeramptrafficpolicyinstancetypetrafficpolicyinstancetypemarker-get
  description: 'Gets information about the traffic policy instances that you created
    by using thecurrent AWS account.NoteAfter you submit an UpdateTrafficPolicyInstance
    request, there''s a briefdelay while Amazon Route 53 creates the resource record
    sets that are specified in the traffic policydefinition. For more information,
    see the State response element.Send a GET request to the /Amazon Route 53 APIversion/trafficpolicyinstance
    resource.Amazon Route 53 returns a maximum of 100 items in each response. If you
    have a lot of trafficpolicy instances, you can use the MaxItems parameter to list
    them in groups of upto 100.The response includes five values that help you navigate
    from one group ofMaxItems traffic policy instances to the next:             IsTruncated           If
    the value of IsTruncated in the response is true,there are more traffic policy
    instances associated with the current AWSaccount.If IsTruncated is false, this
    response includes the lasttraffic policy instance that is associated with the
    current account.             MaxItems           The value that you specified for
    the MaxItems parameter in the requestthat produced the current response.                  HostedZoneIdMarker,
    TrafficPolicyInstanceNameMarker, and TrafficPolicyInstanceTypeMarker               If
    IsTruncated is true, these three values in theresponse represent the first traffic
    policy instance in the next group ofMaxItems traffic policy instances. To list
    more traffic policy instances,make another call to ListTrafficPolicyInstances,
    and specify these values inthe corresponding request parameters.If IsTruncated
    is false, all three elements are omittedfrom the response.'
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/Networking_AmazonRoute53.png
  humanURL: https://aws.amazon.com/route53/
  baseURL: :///
  tags: Amazon Web Services, DNS, API Service Provider, API Service Provider, API
    Provider, Profiles, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/items/master/_listings/aws-route-53/20130401trafficpolicyinstanceshostedzoneidhostedzoneidmarkerampmaxitemsmaxitemsamptrafficpolicyinstancenametrafficpolicyinstancenamemarkeramptrafficpolicyinstancetypetrafficpolicyinstancetypemarker-get-openapi.md
x-common:
- type: x-api-gallery
  url: http://aws.rekognition.api.gallery.streamdata.io
- type: x-api-stack
  url: http://aws.route.53.stack.network
- type: x-documentation
  url: http://docs.aws.amazon.com/Route53/latest/APIReference/
- type: x-faq
  url: https://aws.amazon.com/route53/faqs/
- type: x-forum
  url: https://forums.aws.amazon.com/forum.jspa?forumID=87
- type: x-pricing
  url: https://aws.amazon.com/route53/pricing/
- type: x-registrar-policies
  url: https://aws.amazon.com/route53/amazon-registrar-policies/
- type: x-service-health
  url: http://status.aws.amazon.com/
- type: x-service-level-agreement
  url: https://aws.amazon.com/route53/sla
- type: x-sla
  url: https://aws.amazon.com/route53/sla/
- type: x-website
  url: https://aws.amazon.com/route53/
include: []
maintainers:
- FN: Kin Lane
  x-twitter: apievangelist
  email: info@apievangelist.com
---