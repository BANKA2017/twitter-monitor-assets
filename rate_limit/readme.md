# Rate limit checker

---

- The number is the number of rate limit, and `_` means response headers have no field `x-rate-limit-limit`
- ❌ means the endpoint is unavailable

## Graphql

|                               |            old web |            new web |  tweetdeck preview |            android |       real account |             cookie|
| :-- | --: | --: | --: | --: | --: | --: |
| graphql:userinfo_screen_name    |            150 ✅ |            150 ❌ |            150 ✅ |            150 ✅ |            150 ✅ |              _ ❌ |
| graphql:userinfo_uid            |            500 ✅ |            500 ❌ |            500 ✅ |            500 ✅ |            500 ✅ |              _ ❌ |
| graphql:tweets_web              |             50 ✅ |             50 ✅ |            800 ✅ |             50 ✅ |             50 ✅ |              _ ❌ |
| graphql:tweets_with_replies_web |            500 ✅ |            500 ❌ |            500 ✅ |            500 ✅ |            500 ✅ |              _ ❌ |
| graphql:tweets_v2               |            500 ❌ |            500 ❌ |            500 ❌ |            500 ❌ |            500 ✅ |              _ ❌ |
| graphql:tweets_with_replies_v2  |            500 ❌ |            500 ❌ |            500 ❌ |            500 ❌ |            500 ✅ |              _ ❌ |
| graphql:conversation            |            150 ❌ |            150 ❌ |            150 ❌ |            150 ❌ |            150 ✅ |              _ ❌ |
| graphql:conversation_v2         |            500 ❌ |            500 ❌ |            500 ❌ |              _ ❌ |            500 ✅ |              _ ❌ |
| graphql:tweet_result_by_id      |             50 ✅ |             50 ✅ |            300 ✅ |             50 ✅ |             50 ✅ |              _ ❌ |
| graphql:search                  |              _ ❌ |              _ ❌ |              _ ❌ |              _ ❌ |              _ ❌ |              _ ❌ |
| graphql:search_client           |              _ ❌ |              _ ❌ |              _ ❌ |              _ ❌ |              _ ❌ |              _ ❌ |
| graphql:edit_history            |            500 ❌ |            500 ❌ |            500 ❌ |              _ ❌ |              _ ❌ |              _ ❌ |
| graphql:audiospace              |            500 ✅ |            500 ✅ |            500 ✅ |              _ ❌ |            500 ✅ |              _ ❌ |
| graphql:translate_bio           |              _ ❌ |              _ ❌ |              _ ❌ |              _ ❌ |              _ ❌ |              _ ❌ |
| graphql:translate_tweet         |            500 ❌ |            500 ❌ |            500 ❌ |              _ ❌ |            500 ✅ |              _ ❌ |
| graphql:list_info               |            500 ❌ |            500 ❌ |            500 ❌ |              _ ❌ |            500 ✅ |              _ ❌ |
| graphql:list_member             |            500 ❌ |            500 ❌ |            500 ❌ |              _ ❌ |            500 ✅ |              _ ❌ |
| graphql:list_timeline           |            500 ❌ |            500 ❌ |           1000 ❌ |              _ ❌ |            500 ✅ |              _ ❌ |
| graphql:community_info          |             50 ✅ |             50 ✅ |             50 ✅ |              _ ❌ |             50 ✅ |              _ ❌ |
| graphql:community_search        |            500 ❌ |            500 ❌ |            500 ❌ |              _ ❌ |            500 ✅ |              _ ❌ |
| graphql:community_timeline      |            500 ❌ |            500 ❌ |            500 ❌ |              _ ❌ |            500 ✅ |              _ ❌ |

## Restful

|                               |            old web |            new web |  tweetdeck preview |            android |       real account |             cookie|
| :-- | --: | --: | --: | --: | --: | --: |
| restful:userinfo_screen_name    |            180 ❌ |            180 ❌ |            180 ❌ |            180 ❌ |            900 ✅ |              _ ❌ |
| restful:userinfo_uid            |            180 ❌ |            180 ❌ |            180 ❌ |            180 ❌ |            900 ✅ |              _ ❌ |
| restful:tweets                  |            300 ❌ |            300 ❌ |            300 ❌ |            300 ❌ |            180 ❌ |              _ ❌ |
| restful:conversation            |            180 ❌ |            180 ❌ |            180 ❌ |              _ ❌ |            180 ✅ |              _ ❌ |
| restful:search                  |              _ ❌ |              _ ❌ |              _ ❌ |              _ ❌ |              _ ❌ |              _ ❌ |
| restful:broadcast               |              _ ✅ |              _ ✅ |              _ ✅ |              _ ❌ |              _ ❌ |              _ ❌ |
| restful:live_stream             |              _ ✅ |              _ ✅ |              _ ✅ |              _ ❌ |              _ ❌ |              _ ❌ |
| restful:typeahead               |              _ ❌ |              _ ❌ |              _ ❌ |              _ ❌ |              _ ✅ |              _ ❌ |
| restful:trends                  |          20000 ❌ |          20000 ❌ |          20000 ❌ |              _ ❌ |          20000 ✅ |              _ ❌ |
| restful:translate_bio           |            187 ❌ |            187 ❌ |            187 ✅ |              _ ❌ |              _ ❌ |              _ ❌ |
| restful:translate_tweet         |            187 ❌ |            187 ❌ |            187 ❌ |              _ ❌ |              _ ❌ |              _ ❌ |
| restful:list_timeline           |            180 ❌ |            180 ❌ |            180 ❌ |              _ ❌ |           1800 ❌ |              _ ❌ |
| restful:following               |            187 ✅ |            180 ✅ |            180 ✅ |              _ ❌ |            180 ✅ |              _ ❌ |
| restful:followers               |             15 ✅ |             15 ✅ |             15 ✅ |              _ ❌ |            180 ✅ |              _ ❌ |
| restful:likes                   |            187 ❌ |            180 ❌ |            180 ❌ |              _ ❌ |             75 ❌ |              _ ❌ |
| restful:onbroading              |            187 ✅ |            187 ✅ |            187 ✅ |              _ ❌ |            187 ✅ |              _ ❌ |

><https://github.com/BANKA2017/twitter-monitor/tree/node/apps/rate_limit_checker>

- Now everyone can embed broadcast players directly, so the rate limit of the broadcast endpoint can be regarded as none [[original tweet](https://twitter.com/Live/status/1733197678706852095)]
- All guest accounts were expired, we have to remove them
- The *real account* registered on 2023-06
