# Rate limit checker

---

- The number is the number of rate limit, and `_` means response headers have no field `x-rate-limit-limit`
- ❌ means the endpoint is unavailable

## Graphql

|                               |            old web |            new web |  tweetdeck preview |      guest account|
| :-- | --: | --: | --: | --: |
| graphql:userinfo_screen_name    |             95 ✅ |             95 ✅ |             95 ✅ |             95 ✅ |
| graphql:userinfo_uid            |            500 ❌ |            500 ❌ |            500 ❌ |            500 ✅ |
| graphql:tweets_web              |             50 ✅ |             50 ✅ |            800 ✅ |             50 ✅ |
| graphql:tweets_with_replies_web |             50 ❌ |             50 ❌ |            300 ❌ |             50 ✅ |
| graphql:tweets_v2               |            500 ❌ |            500 ❌ |            500 ❌ |            500 ✅ |
| graphql:tweets_with_replies_v2  |            500 ❌ |            500 ❌ |            500 ❌ |            500 ✅ |
| graphql:conversation            |            150 ❌ |            150 ❌ |            150 ❌ |            150 ✅ |
| graphql:conversation_v2         |            500 ❌ |            500 ❌ |            500 ❌ |            500 ✅ |
| graphql:tweet_result_by_id      |             50 ✅ |             50 ✅ |            300 ✅ |             50 ✅ |
| graphql:search                  |             50 ❌ |             50 ❌ |           1200 ❌ |             50 ✅ |
| graphql:search_client           |             50 ❌ |             50 ❌ |           1200 ❌ |             50 ✅ |
| graphql:edit_history            |            500 ❌ |            500 ❌ |            500 ❌ |            500 ✅ |
| graphql:audiospace              |            500 ❌ |            500 ❌ |            500 ❌ |            500 ✅ |
| graphql:translate_bio           |              _ ❌ |              _ ❌ |              _ ❌ |              _ ❌ |
| graphql:translate_tweet         |            500 ❌ |            500 ❌ |            500 ❌ |            500 ✅ |
| graphql:list_info               |            500 ❌ |            500 ❌ |            500 ❌ |            500 ✅ |
| graphql:list_member             |            500 ❌ |            500 ❌ |            500 ❌ |            500 ✅ |
| graphql:list_timeline           |            500 ❌ |            500 ❌ |           1000 ❌ |            500 ✅ |
| graphql:community_info          |            500 ❌ |            500 ❌ |            500 ❌ |            500 ✅ |
| graphql:community_search        |            500 ❌ |            500 ❌ |            500 ❌ |            500 ✅ |
| graphql:community_timeline      |            500 ❌ |            500 ❌ |            500 ❌ |            500 ✅ |

## Restful

|                               |            old web |            new web |  tweetdeck preview |      guest account|
| :-- | --: | --: | --: | --: |
| restful:userinfo_screen_name    |            180 ❌ |            180 ❌ |            180 ❌ |            900 ✅ |
| restful:userinfo_uid            |            180 ❌ |            180 ❌ |            180 ❌ |            900 ✅ |
| restful:tweets                  |            300 ❌ |            300 ❌ |            300 ❌ |            180 ✅ |
| restful:conversation            |            180 ❌ |            180 ❌ |            180 ❌ |            180 ✅ |
| restful:search                  |              _ ❌ |              _ ❌ |              _ ❌ |              _ ✅ |
| restful:broadcast               |            187 ✅ |            187 ✅ |            187 ✅ |            900 ✅ |
| restful:live_stream             |              _ ✅ |              _ ✅ |              _ ✅ |              _ ✅ |
| restful:typeahead               |              _ ❌ |              _ ❌ |              _ ❌ |              _ ✅ |
| restful:trends                  |          20000 ❌ |          20000 ❌ |          20000 ❌ |          20000 ✅ |
| restful:translate_bio           |            187 ❌ |            187 ❌ |            187 ❌ |              _ ❌ |
| restful:translate_tweet         |            187 ❌ |            187 ❌ |            187 ❌ |              _ ❌ |
| restful:list_timeline           |            180 ❌ |            180 ❌ |            180 ❌ |           1800 ✅ |
| restful:following               |            187 ✅ |            180 ✅ |            180 ✅ |            180 ✅ |
| restful:followers               |             15 ✅ |             15 ✅ |             15 ✅ |            180 ✅ |
| restful:likes                   |            187 ❌ |            180 ❌ |            180 ❌ |             75 ✅ |
| restful:onbroading              |            187 ✅ |            187 ✅ |            187 ✅ |            187 ✅ |

><https://github.com/BANKA2017/twitter-monitor/tree/node/apps/rate_limit_checker>
