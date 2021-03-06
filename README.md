# Query the project

````graphql
query {
  councillors(first: 5, orderBy: NUMBER_OF_VOTES_DESC) {
    nodes {
      id
      numberOfVotes
      voteHistory(first: 3) {
        totalCount
        nodes {
          approvedVote
        }
      }
    }
  }
}
````

# Output

````json
{
  "data": {
    "councillors": {
      "nodes": [
        {
          "id": "12hAtDZJGt4of3m2GqZcUCVAjZPALfvPwvtUTFZPQUbdX1Ud",
          "numberOfVotes": 50,
          "voteHistory": {
            "totalCount": 50,
            "nodes": [
              {
                "approvedVote": true
              },
              {
                "approvedVote": true
              },
              {
                "approvedVote": true
              }
            ]
          }
        },
        {
          "id": "1363HWTPzDrzAQ6ChFiMU6mP4b6jmQid2ae55JQcKtZnpLGv",
          "numberOfVotes": 46,
          "voteHistory": {
            "totalCount": 46,
            "nodes": [
              {
                "approvedVote": true
              },
              {
                "approvedVote": true
              },
              {
                "approvedVote": true
              }
            ]
          }
        },
        {
          "id": "12NLgzqfhuJkc9mZ5XUTTG85N8yhhzfptwqF1xVhtK3ZX7f6",
          "numberOfVotes": 45,
          "voteHistory": {
            "totalCount": 45,
            "nodes": [
              {
                "approvedVote": true
              },
              {
                "approvedVote": true
              },
              {
                "approvedVote": true
              }
            ]
          }
        },
        {
          "id": "12Y8b4C9ar162cBgycxYgxxHG7cLVs8gre9Y5xeMjW3izqer",
          "numberOfVotes": 44,
          "voteHistory": {
            "totalCount": 44,
            "nodes": [
              {
                "approvedVote": true
              },
              {
                "approvedVote": true
              },
              {
                "approvedVote": true
              }
            ]
          }
        },
        {
          "id": "16UJBPHVqQ3xYXnmhEpaQtvSRnrP9k1XeE7WxoyCxsrL9AvV",
          "numberOfVotes": 41,
          "voteHistory": {
            "totalCount": 41,
            "nodes": [
              {
                "approvedVote": true
              },
              {
                "approvedVote": true
              },
              {
                "approvedVote": true
              }
            ]
          }
        }
      ]
    }
  }
}
````