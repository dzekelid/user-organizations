{
  "info": {
    "name": "CloudFlare Get a specific organization the user is associated with",
    "_postman_id": "4ec5a644-3876-44d0-82c1-c30b1cf65084",
    "description": "Get a specific organization the user is associated with",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Subscriptions",
      "item": [
        {
          "id": "ef581562-26a7-441a-b915-f708fffdd5ff",
          "name": "cloudflare-app-subscription-api",
          "request": {
            "url": "http://example.com/api/user/billing/subscriptions/apps?activated_on=%7B%7D&cancelled_on=%7B%7D&direction=%7B%7D&expired_on=%7B%7D&expires_on=%7B%7D&match=%7B%7D&order=%7B%7D&page=%7B%7D&per_page=%7B%7D&price=%7B%7D&renewed_on=%7B%7D&status=%7B%7D",
            "method": "GET",
            "header": [
              {
                "key": "X-AUTH-EMAIL",
                "value": "{}",
                "description": "Email address associated with your account",
                "disabled": false
              },
              {
                "key": "X-AUTH-KEY",
                "value": "{}",
                "description": "API key generated on the My Account page",
                "disabled": false
              }
            ],
            "body": {
              "mode": "raw"
            },
            "description": "List all of your app subscriptions"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "83d03aae-7fa0-4cda-aa5c-d93fa83104fc"
            }
          ]
        },
        {
          "id": "b09d03ae-6ff6-4188-b9a2-d38a62f41289",
          "name": "cloudflare-app-subscription-api",
          "request": {
            "url": "http://example.com/api/user/billing/subscriptions/apps/:identifier",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Billing subscription details"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "c55c7380-9732-4c91-9aba-ac393b82c14a"
            }
          ]
        }
      ]
    },
    {
      "name": "Zones",
      "item": [
        {
          "id": "9e82d2cc-7212-4941-a876-66d92f2329e0",
          "name": "cloudflare-custom-pages-for-a-zone-api",
          "request": {
            "url": "http://example.com/api/zones/:zone_identifier/custom_pages",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "A list of available Custom Pages the zone can use"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "546d9c7e-b360-4a02-b173-af27aeee2b0f"
            }
          ]
        },
        {
          "id": "c96b2f17-1b57-444d-a36a-edb749c3beb4",
          "name": "cloudflare-custom-pages-for-a-zone-api1",
          "request": {
            "url": "http://example.com/api/zones/:zone_identifier/custom_pages/:identifier",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Details about a specific Custom page details"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "064d0cb8-e115-40d2-aea6-bf3ebf77c6a2"
            }
          ]
        },
        {
          "id": "c3726bbf-da5a-411a-b63f-37824bbf94cf",
          "name": "cloudflare-custom-pages-for-a-zone-api",
          "request": {
            "url": "http://example.com/api/zones/:zone_identifier/custom_pages/:identifier?state=%7B%7D&url=%7B%7D",
            "method": "PUT",
            "header": [
              {
                "key": "X-AUTH-EMAIL",
                "value": "{}",
                "description": "Email address associated with your account",
                "disabled": false
              },
              {
                "key": "X-AUTH-KEY",
                "value": "{}",
                "description": "API key generated on the My Account page",
                "disabled": false
              }
            ],
            "body": {
              "mode": "raw"
            },
            "description": "Update Custom page URL"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "746097a1-e4b7-4f5e-9c38-e8c2cef9f717"
            }
          ]
        }
      ]
    },
    {
      "name": "Certificates",
      "item": [
        {
          "id": "90f74e68-6c1b-4029-be6d-2e34f5d0ccb3",
          "name": "cloudflare-custom-ssl-for-a-zone-api",
          "request": {
            "url": "http://example.com/api/zones/:zone_identifier/custom_certificates?direction=%7B%7D&match=%7B%7D&order=%7B%7D&page=%7B%7D&per_page=%7B%7D&status=%7B%7D",
            "method": "GET",
            "header": [
              {
                "key": "X-AUTH-EMAIL",
                "value": "{}",
                "description": "Email address associated with your account",
                "disabled": false
              },
              {
                "key": "X-AUTH-KEY",
                "value": "{}",
                "description": "API key generated on the My Account page",
                "disabled": false
              }
            ],
            "body": {
              "mode": "raw"
            },
            "description": "List, search, sort, and filter all of your custom SSL certificates"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "9f6c46e9-eebb-468c-8a2c-785fd041356b"
            }
          ]
        },
        {
          "id": "49062f48-2ed1-444a-a3c1-9d02abf30a6d",
          "name": "cloudflare-custom-ssl-for-a-zone-api",
          "request": {
            "url": "http://example.com/api/zones/:zone_identifier/custom_certificates?certificate=%7B%7D&private_key=%7B%7D",
            "method": "POST",
            "header": [
              {
                "key": "X-AUTH-EMAIL",
                "value": "{}",
                "description": "Email address associated with your account",
                "disabled": false
              },
              {
                "key": "X-AUTH-KEY",
                "value": "{}",
                "description": "API key generated on the My Account page",
                "disabled": false
              }
            ],
            "body": {
              "mode": "raw"
            },
            "description": "Upload a new SSL certificate for a zone"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "fdaeb763-e02b-40f3-894c-dd38564c6cfd"
            }
          ]
        },
        {
          "id": "3df435ca-3417-44df-9fbe-cdc8d8bff90f",
          "name": "cloudflare-custom-ssl-for-a-zone-api",
          "request": {
            "url": "http://example.com/api/zones/:zone_identifier/custom_certificates/:identifier",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "SSL configuration details permission needed: #ssl:readntt"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "2c35527d-4143-4f05-8fed-0bdac37ce7cb"
            }
          ]
        },
        {
          "id": "ae62d3dd-f3d0-4cc6-90d9-0821c1fc5ddd",
          "name": "cloudflare-custom-ssl-for-a-zone-api",
          "request": {
            "url": "http://example.com/api/zones/:zone_identifier/custom_certificates/:identifier",
            "method": "DELETE",
            "body": {
              "mode": "raw"
            },
            "description": "Delete an SSL certificate permission needed: #ssl:editntt"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "81a719ed-158a-4c91-b8bf-483a84425e56"
            }
          ]
        },
        {
          "id": "d6298a02-dcc3-4bb6-bdc6-2dc1e67ce459",
          "name": "cloudflare-custom-ssl-for-a-zone-api",
          "request": {
            "url": "http://example.com/api/zones/:zone_identifier/custom_certificates/:identifier?certificate=%7B%7D&private_key=%7B%7D",
            "method": "PATCH",
            "header": [
              {
                "key": "X-AUTH-EMAIL",
                "value": "{}",
                "description": "Email address associated with your account",
                "disabled": false
              },
              {
                "key": "X-AUTH-KEY",
                "value": "{}",
                "description": "API key generated on the My Account page",
                "disabled": false
              }
            ],
            "body": {
              "mode": "raw"
            },
            "description": "Upload a new private key and/or PEM/CRT for the SSL certificate"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "4be12a69-cc1e-4798-956a-c40a32d1e708"
            }
          ]
        },
        {
          "id": "2b273a0a-3635-4e42-8729-c8fa256cc524",
          "name": "cloudflare-custom-ssl-for-a-zone-api",
          "request": {
            "url": "http://example.com/api/zones/:zone_identifier/custom_certificates/prioritize?certificates=%7B%7D",
            "method": "PUT",
            "header": [
              {
                "key": "X-AUTH-EMAIL",
                "value": "{}",
                "description": "Email address associated with your account",
                "disabled": false
              },
              {
                "key": "X-AUTH-KEY",
                "value": "{}",
                "description": "API key generated on the My Account page",
                "disabled": false
              }
            ],
            "body": {
              "mode": "raw"
            },
            "description": "If a zone has multiple SSL certificates, you can set the order in which they should be used during a request"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "850a2543-6587-4970-bc99-4cf9fdf95997"
            }
          ]
        }
      ]
    },
    {
      "name": "Records",
      "item": [
        {
          "id": "bfe8f97b-9d70-470b-9469-2221e40bd1d3",
          "name": "cloudflare-dns-records-for-a-zone-api",
          "request": {
            "url": "http://example.com/api/zones/:zone_identifier/dns_records?content=%7B%7D&direction=%7B%7D&match=%7B%7D&name=%7B%7D&order=%7B%7D&page=%7B%7D&per_page=%7B%7D&type=%7B%7D",
            "method": "GET",
            "header": [
              {
                "key": "X-AUTH-EMAIL",
                "value": "{}",
                "description": "Email address associated with your account",
                "disabled": false
              },
              {
                "key": "X-AUTH-KEY",
                "value": "{}",
                "description": "API key generated on the My Account page",
                "disabled": false
              }
            ],
            "body": {
              "mode": "raw"
            },
            "description": "List, search, sort, and filter a zones&#39; DNS records"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "9005402d-16bd-4d50-9bf1-e6dc3d1a4280"
            }
          ]
        },
        {
          "id": "8ab301df-5a77-4f75-aafa-977689e41aa2",
          "name": "cloudflare-dns-records-for-a-zone-api",
          "request": {
            "url": "http://example.com/api/zones/:zone_identifier/dns_records?content=%7B%7D&name=%7B%7D&type=%7B%7D",
            "method": "POST",
            "header": [
              {
                "key": "X-AUTH-EMAIL",
                "value": "{}",
                "description": "Email address associated with your account",
                "disabled": false
              },
              {
                "key": "X-AUTH-KEY",
                "value": "{}",
                "description": "API key generated on the My Account page",
                "disabled": false
              }
            ],
            "body": {
              "mode": "raw"
            },
            "description": "Create a new DNS record for a zone"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "a094f813-114b-4677-aff1-00f48fd0b835"
            }
          ]
        },
        {
          "id": "42518860-1b56-4e3f-bcf7-45fdd608ae9a",
          "name": "cloudflare-dns-records-for-a-zone-api",
          "request": {
            "url": "http://example.com/api/zones/:zone_identifier/dns_records/:identifier",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "DNS record details permission needed: #dns_records:readntt"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "394f06e1-ae17-4026-b9f7-d7719f70aad3"
            }
          ]
        },
        {
          "id": "01b77760-988a-4971-92c1-f86e922d319e",
          "name": "cloudflare-dns-records-for-a-zone-api",
          "request": {
            "url": "http://example.com/api/zones/:zone_identifier/dns_records/:identifier",
            "method": "PUT",
            "body": {
              "mode": "raw"
            },
            "description": "Update DNS record permission needed: #dns_records:editntt"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "36d0c511-030d-4bfa-b9aa-126a58189bcc"
            }
          ]
        },
        {
          "id": "318e5e59-7bdb-41e1-8cb2-b4d0808316e9",
          "name": "cloudflare-dns-records-for-a-zone-api",
          "request": {
            "url": "http://example.com/api/zones/:zone_identifier/dns_records/:identifier",
            "method": "DELETE",
            "body": {
              "mode": "raw"
            },
            "description": "Delete DNS record permission needed: #dns_records:editntt"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "76764463-2c69-46a6-a019-6b87e10400ef"
            }
          ]
        }
      ]
    },
    {
      "name": "Firewall Access Rule",
      "item": [
        {
          "id": "c647a1ab-cdb0-4f82-a91a-59eb631d1de1",
          "name": "cloudflare-firewall-access-rule-for-a-zone-api",
          "request": {
            "url": "http://example.com/api/zones/:zone_id/firewall/access_rules/rules?configuration_target=%7B%7D&configuration_value=%7B%7D&direction=%7B%7D&match=%7B%7D&mode=%7B%7D&order=%7B%7D&page=%7B%7D&per_page=%7B%7D&scope_type=%7B%7D",
            "method": "GET",
            "header": [
              {
                "key": "X-AUTH-EMAIL",
                "value": "{}",
                "description": "Email address associated with your account",
                "disabled": false
              },
              {
                "key": "X-AUTH-KEY",
                "value": "{}",
                "description": "API key generated on the My Account page",
                "disabled": false
              }
            ],
            "body": {
              "mode": "raw"
            },
            "description": "Search, sort, and filter IP/country access rules"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "94367c48-eb1e-4082-be86-460aa0f06540"
            }
          ]
        },
        {
          "id": "2288ad4e-a6e9-4aa6-ae80-95ba13c95a3b",
          "name": "cloudflare-firewall-access-rule-for-a-zone-api",
          "request": {
            "url": "http://example.com/api/zones/:zone_id/firewall/access_rules/rules?configuration=%7B%7D&mode=%7B%7D&value=%7B%7D",
            "method": "POST",
            "header": [
              {
                "key": "X-AUTH-EMAIL",
                "value": "{}",
                "description": "Email address associated with your account",
                "disabled": false
              },
              {
                "key": "X-AUTH-KEY",
                "value": "{}",
                "description": "API key generated on the My Account page",
                "disabled": false
              }
            ],
            "body": {
              "mode": "raw"
            },
            "description": "Make a new IP, IP range, or country access rule for the zone"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "0f7e3b26-02f2-4632-b892-f4fbdfade00b"
            }
          ]
        },
        {
          "id": "1cc57756-4266-4fea-a612-cf2085ca70da",
          "name": "cloudflare-firewall-access-rule-for-a-zone-api",
          "request": {
            "url": "http://example.com/api/zones/:zone_id/firewall/access_rules/rules/:identifier?cascade=%7B%7D",
            "method": "DELETE",
            "header": [
              {
                "key": "X-AUTH-EMAIL",
                "value": "{}",
                "description": "Email address associated with your account",
                "disabled": false
              },
              {
                "key": "X-AUTH-KEY",
                "value": "{}",
                "description": "API key generated on the My Account page",
                "disabled": false
              }
            ],
            "body": {
              "mode": "raw"
            },
            "description": "Remove an access rule so it is no longer evaluated during requests"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "082b35ac-fe7a-4784-862c-d03f021513bb"
            }
          ]
        },
        {
          "id": "ca84052e-6180-4e5e-9749-1c2a8a6e201a",
          "name": "cloudflare-firewall-access-rule-for-a-zone-api",
          "request": {
            "url": "http://example.com/api/zones/:zone_id/firewall/access_rules/rules/:identifier?mode=%7B%7D&notes=%7B%7D",
            "method": "PATCH",
            "header": [
              {
                "key": "X-AUTH-EMAIL",
                "value": "{}",
                "description": "Email address associated with your account",
                "disabled": false
              },
              {
                "key": "X-AUTH-KEY",
                "value": "{}",
                "description": "API key generated on the My Account page",
                "disabled": false
              }
            ],
            "body": {
              "mode": "raw"
            },
            "description": "Update rule state and/or configuration for the zone"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "6d1d0db5-5f79-4bd6-a1b3-d356631e47ca"
            }
          ]
        }
      ]
    },
    {
      "name": "Keyless Certificates",
      "item": [
        {
          "id": "090b900a-8aa6-4700-adb3-59ffd7ea0e8f",
          "name": "cloudflare-keyless-ssl-for-a-zone-api",
          "request": {
            "url": "http://example.com/api/zones/:zone_identifier/keyless_certificates",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "List all Keyless SSL configurations for a given zone"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "5eb4174c-0f7c-4086-8d00-7bde91259cff"
            }
          ]
        },
        {
          "id": "adeba62c-6fb6-4034-9294-3ba5aa45d114",
          "name": "cloudflare-keyless-ssl-for-a-zone-api",
          "request": {
            "url": "http://example.com/api/zones/:zone_identifier/keyless_certificates?certificate=%7B%7D&host=%7B%7D&name=%7B%7D&port=%7B%7D",
            "method": "POST",
            "header": [
              {
                "key": "X-AUTH-EMAIL",
                "value": "{}",
                "description": "Email address associated with your account",
                "disabled": false
              },
              {
                "key": "X-AUTH-KEY",
                "value": "{}",
                "description": "API key generated on the My Account page",
                "disabled": false
              }
            ],
            "body": {
              "mode": "raw"
            },
            "description": "The keyless SSL name"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "75588676-e7fc-4faf-82ca-f475805fc16a"
            }
          ]
        },
        {
          "id": "1e45d80d-f57e-4fad-91b9-ba1b600639ed",
          "name": "cloudflare-keyless-ssl-for-a-zone-api1",
          "request": {
            "url": "http://example.com/api/zones/:zone_identifier/keyless_certificates/:identifier",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Details for one Keyless SSL configuration"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "c01344b9-74ea-4a77-95c7-d4be7fe4bfd0"
            }
          ]
        },
        {
          "id": "6d1cda4c-1d06-445f-8e01-727024a28d3f",
          "name": "cloudflare-keyless-ssl-for-a-zone-api",
          "request": {
            "url": "http://example.com/api/zones/:zone_identifier/keyless_certificates/:identifier",
            "method": "DELETE",
            "body": {
              "mode": "raw"
            },
            "description": "Delete Keyless configuration permission needed: #ssl:editntt"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "eba24bb7-d682-4d9a-bd30-3f5a1edbad6c"
            }
          ]
        },
        {
          "id": "a131b94d-e30d-4b1e-b4e0-9315d94899bc",
          "name": "cloudflare-keyless-ssl-for-a-zone-api",
          "request": {
            "url": "http://example.com/api/zones/:zone_identifier/keyless_certificates/:identifier?host=%7B%7D&name=%7B%7D&port=%7B%7D",
            "method": "PATCH",
            "header": [
              {
                "key": "X-AUTH-EMAIL",
                "value": "{}",
                "description": "Email address associated with your account",
                "disabled": false
              },
              {
                "key": "X-AUTH-KEY",
                "value": "{}",
                "description": "API key generated on the My Account page",
                "disabled": false
              }
            ],
            "body": {
              "mode": "raw"
            },
            "description": "This will update attributes of a Keyless SSL"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "3d1e372e-b836-4064-bd7f-19c658b321a2"
            }
          ]
        }
      ]
    },
    {
      "name": "Organization Invites",
      "item": [
        {
          "id": "27defb8a-85d3-4ad5-9415-b73c03304d00",
          "name": "cloudflare-organization-invites-api",
          "request": {
            "url": "http://example.com/api/organizations/:organization_identifier/invite/:identifier?roles=%7B%7D",
            "method": "PATCH",
            "header": [
              {
                "key": "X-AUTH-EMAIL",
                "value": "{}",
                "description": "Email address associated with your account",
                "disabled": false
              },
              {
                "key": "X-AUTH-KEY",
                "value": "{}",
                "description": "API key generated on the My Account page",
                "disabled": false
              }
            ],
            "body": {
              "mode": "raw"
            },
            "description": "Change the Roles of a Pending Invite"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "e2b791c7-38b9-42fb-b1f1-2a43edeb5619"
            }
          ]
        },
        {
          "id": "173cf875-d12f-4127-a33a-5e693f6e28db",
          "name": "cloudflare-organization-invites-api",
          "request": {
            "url": "http://example.com/api/organizations/:organization_identifier/invites",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "List all invitations associated with an organization"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "b4581b4b-4ff1-4494-a5a2-9999fe913a02"
            }
          ]
        },
        {
          "id": "2bb82753-6b7e-48e6-83c3-ca6e709bcdb0",
          "name": "cloudflare-organization-invites-api",
          "request": {
            "url": "http://example.com/api/organizations/:organization_identifier/invites?invited_member_email=%7B%7D&roles=%7B%7D",
            "method": "POST",
            "header": [
              {
                "key": "X-AUTH-EMAIL",
                "value": "{}",
                "description": "Email address associated with your account",
                "disabled": false
              },
              {
                "key": "X-AUTH-KEY",
                "value": "{}",
                "description": "API key generated on the My Account page",
                "disabled": false
              }
            ],
            "body": {
              "mode": "raw"
            },
            "description": "Invite a User to become a Member of an Organization"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "f317a4c4-9108-4fb8-8bbc-dbe4334e0471"
            }
          ]
        },
        {
          "id": "2cdce4d2-cbe1-49db-9679-f466b9124b4e",
          "name": "cloudflare-organization-invites-api1",
          "request": {
            "url": "http://example.com/api/organizations/:organization_identifier/invites/:identifier",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Get the details of an invitation"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "17b4edf7-3f7b-4037-9552-6eee766981a4"
            }
          ]
        },
        {
          "id": "c64c501e-c7c7-4a89-b28e-80cd9ae8bfd9",
          "name": "cloudflare-organization-invites-api",
          "request": {
            "url": "http://example.com/api/organizations/:organization_identifier/invites/:identifier",
            "method": "DELETE",
            "body": {
              "mode": "raw"
            },
            "description": "Cancel an existing invitation"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "88c309d9-c3b1-4f03-9113-1995190d0515"
            }
          ]
        }
      ]
    },
    {
      "name": "Organization Members",
      "item": [
        {
          "id": "5d761196-c1f8-4b26-80dc-c809ef8f32b6",
          "name": "cloudflare-organization-members-api",
          "request": {
            "url": "http://example.com/api/organizations/:organization_identifier/members",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "List all members of a organization"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "17a3f679-b836-4a42-82bf-7042906c9052"
            }
          ]
        },
        {
          "id": "e49c3edc-66cd-4dd2-a961-1a728ae7dd51",
          "name": "cloudflare-organization-members-api1",
          "request": {
            "url": "http://example.com/api/organizations/:organization_identifier/members/:identifier",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Get information about a specific member of an organization"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "86b33821-bc2b-4721-bef4-65f294cbeb65"
            }
          ]
        },
        {
          "id": "019d8608-dc61-4c7f-a040-de19777c9b90",
          "name": "cloudflare-organization-members-api",
          "request": {
            "url": "http://example.com/api/organizations/:organization_identifier/members/:identifier",
            "method": "DELETE",
            "body": {
              "mode": "raw"
            },
            "description": "Remove a member from an organization"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "5eb7d874-8bce-4403-9aa2-eefc8291fbfb"
            }
          ]
        },
        {
          "id": "a009c344-8ace-44f9-9a36-174992630304",
          "name": "cloudflare-organization-members-api",
          "request": {
            "url": "http://example.com/api/organizations/:organization_identifier/members/:identifier?roles=%7B%7D",
            "method": "PATCH",
            "header": [
              {
                "key": "X-AUTH-EMAIL",
                "value": "{}",
                "description": "Email address associated with your account",
                "disabled": false
              },
              {
                "key": "X-AUTH-KEY",
                "value": "{}",
                "description": "API key generated on the My Account page",
                "disabled": false
              }
            ],
            "body": {
              "mode": "raw"
            },
            "description": "Change the Roles of an Organization&#39;s Member"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "51d70461-be52-4070-a02a-fa389e362b28"
            }
          ]
        }
      ]
    },
    {
      "name": "Organization Roles",
      "item": [
        {
          "id": "7aa9535c-8cda-4f73-bcd5-9a133ae5f779",
          "name": "cloudflare-organization-roles-api",
          "request": {
            "url": "http://example.com/api/organizations/:organization_identifier/roles",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Get all available roles for an organization"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "4b5053a3-7c6d-4438-a7ff-40636b36ed6e"
            }
          ]
        },
        {
          "id": "f05461ee-5294-437a-8360-962675a8a12c",
          "name": "cloudflare-organization-roles-api1",
          "request": {
            "url": "http://example.com/api/organizations/:organization_identifier/roles/:identifier",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Get information about a specific role for an organization"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "f99103a2-8d58-4913-bb76-f5559ec48118"
            }
          ]
        }
      ]
    },
    {
      "name": "Organization Firewall Access Rules",
      "item": [
        {
          "id": "9ac320ea-36e7-47aa-a63a-b2954ac8f87b",
          "name": "cloudflare-organizationlevel-firewall-access-rule-api",
          "request": {
            "url": "http://example.com/api/organizations/:organization_id/firewall/access_rules/rules?configuration_target=%7B%7D&configuration_value=%7B%7D&direction=%7B%7D&match=%7B%7D&mode=%7B%7D&order=%7B%7D&page=%7B%7D&per_page=%7B%7D",
            "method": "GET",
            "header": [
              {
                "key": "X-AUTH-EMAIL",
                "value": "{}",
                "description": "Email address associated with your account",
                "disabled": false
              },
              {
                "key": "X-AUTH-KEY",
                "value": "{}",
                "description": "API key generated on the My Account page",
                "disabled": false
              }
            ],
            "body": {
              "mode": "raw"
            },
            "description": "Search, sort, and filter IP/country access rules"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "9b9b8f37-9666-4ca8-be44-633930c595aa"
            }
          ]
        },
        {
          "id": "d7978eee-8afc-47cd-ae24-8fc31054722b",
          "name": "cloudflare-organizationlevel-firewall-access-rule-api",
          "request": {
            "url": "http://example.com/api/organizations/:organization_id/firewall/access_rules/rules?configuration=%7B%7D&mode=%7B%7D&value=%7B%7D",
            "method": "POST",
            "header": [
              {
                "key": "X-AUTH-EMAIL",
                "value": "{}",
                "description": "Email address associated with your account",
                "disabled": false
              },
              {
                "key": "X-AUTH-KEY",
                "value": "{}",
                "description": "API key generated on the My Account page",
                "disabled": false
              }
            ],
            "body": {
              "mode": "raw"
            },
            "description": "Make a new IP, IP range, or country access rule for all zones owned by the organization"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "6a785376-7f7f-4351-9b0e-7bb606e68193"
            }
          ]
        },
        {
          "id": "532274a3-35b9-437b-981d-47df5d4980e1",
          "name": "cloudflare-organizationlevel-firewall-access-rule-api",
          "request": {
            "url": "http://example.com/api/organizations/:organization_id/firewall/access_rules/rules/:identifier",
            "method": "DELETE",
            "body": {
              "mode": "raw"
            },
            "description": "Remove an access rule so it is no longer evaluated during requests"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "3b74b8af-eebb-4920-bdf5-5e1e365438d7"
            }
          ]
        },
        {
          "id": "c42fd0a4-f1e8-47a5-8feb-13ea9e32db89",
          "name": "cloudflare-organizationlevel-firewall-access-rule-api",
          "request": {
            "url": "http://example.com/api/organizations/:organization_id/firewall/access_rules/rules/:identifier?configuration=%7B%7D&mode=%7B%7D&value=%7B%7D",
            "method": "PATCH",
            "header": [
              {
                "key": "X-AUTH-EMAIL",
                "value": "{}",
                "description": "Email address associated with your account",
                "disabled": false
              },
              {
                "key": "X-AUTH-KEY",
                "value": "{}",
                "description": "API key generated on the My Account page",
                "disabled": false
              }
            ],
            "body": {
              "mode": "raw"
            },
            "description": "Update rule state and/or configuration"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "ccd5f41d-f407-485a-906d-2f5cd7d16b06"
            }
          ]
        }
      ]
    },
    {
      "name": "Organizations",
      "item": [
        {
          "id": "e877b207-20b8-4980-815d-6234b4a33f67",
          "name": "cloudflare-organizations-api",
          "request": {
            "url": "http://example.com/api/organizations/:identifier",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Get information about a specific organization that you are a member of"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "a5803a11-d092-4e99-87dc-5a55aaf545a9"
            }
          ]
        },
        {
          "id": "6a636044-5bd9-48c2-b162-cfba6de762a0",
          "name": "cloudflare-organizations-api",
          "request": {
            "url": "http://example.com/api/organizations/:identifier?name=%7B%7D",
            "method": "PATCH",
            "header": [
              {
                "key": "X-AUTH-EMAIL",
                "value": "{}",
                "description": "Email address associated with your account",
                "disabled": false
              },
              {
                "key": "X-AUTH-KEY",
                "value": "{}",
                "description": "API key generated on the My Account page",
                "disabled": false
              }
            ],
            "body": {
              "mode": "raw"
            },
            "description": "Update an existing Organization"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "c9c43a86-c466-47e8-a80f-f08a789e73cd"
            }
          ]
        }
      ]
    },
    {
      "name": "Performance",
      "item": [
        {
          "id": "e0f56754-0c93-4b73-9576-781e011701a4",
          "name": "cloudflare-railgun-api",
          "request": {
            "url": "http://example.com/api/railguns?direction=%7B%7D&page=%7B%7D&per_page=%7B%7D",
            "method": "GET",
            "header": [
              {
                "key": "X-AUTH-EMAIL",
                "value": "{}",
                "description": "Email address associated with your account",
                "disabled": false
              },
              {
                "key": "X-AUTH-KEY",
                "value": "{}",
                "description": "API key generated on the My Account page",
                "disabled": false
              }
            ],
            "body": {
              "mode": "raw"
            },
            "description": "List, search, sort and filter your Railguns"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "fc8a40ef-b9e0-474e-a740-a08973c90f2e"
            }
          ]
        },
        {
          "id": "95bcb603-5449-4cbd-9c02-9a871acd1868",
          "name": "cloudflare-railgun-api",
          "request": {
            "url": "http://example.com/api/railguns?name=%7B%7D",
            "method": "POST",
            "header": [
              {
                "key": "X-AUTH-EMAIL",
                "value": "{}",
                "description": "Email address associated with your account",
                "disabled": false
              },
              {
                "key": "X-AUTH-KEY",
                "value": "{}",
                "description": "API key generated on the My Account page",
                "disabled": false
              }
            ],
            "body": {
              "mode": "raw"
            },
            "description": "Readable identifier of the railgun"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "1a14a1c9-c2f0-4ce1-99ed-6e3878e9c76f"
            }
          ]
        },
        {
          "id": "280d2e45-e480-40cf-aa99-e84b3ae6a738",
          "name": "cloudflare-railgun-api",
          "request": {
            "url": "http://example.com/api/railguns/:identifier",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Railgun detailsntt"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "53a12000-fa76-45e6-91d1-b3f1bb59baa2"
            }
          ]
        },
        {
          "id": "408a6acb-fc8b-4212-aab6-4634aeaee0e6",
          "name": "cloudflare-railgun-api",
          "request": {
            "url": "http://example.com/api/railguns/:identifier",
            "method": "DELETE",
            "body": {
              "mode": "raw"
            },
            "description": "Disable and delete a Railgun"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "58bb60a5-4ec7-412d-a641-c22a1dd1d18f"
            }
          ]
        },
        {
          "id": "2bc83d86-20a9-4bad-b47f-8ba2ab297435",
          "name": "cloudflare-railgun-api",
          "request": {
            "url": "http://example.com/api/railguns/:identifier?enabled=%7B%7D",
            "method": "PATCH",
            "header": [
              {
                "key": "X-AUTH-EMAIL",
                "value": "{}",
                "description": "Email address associated with your account",
                "disabled": false
              },
              {
                "key": "X-AUTH-KEY",
                "value": "{}",
                "description": "API key generated on the My Account page",
                "disabled": false
              }
            ],
            "body": {
              "mode": "raw"
            },
            "description": "Enable or disable a Railgun for all zones connected to it"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "65c3280a-0a38-43f9-a2a6-25d6fa027af9"
            }
          ]
        },
        {
          "id": "ffeaedbb-5f45-45ec-98d3-61c3f804b7dc",
          "name": "cloudflare-railgun-api1",
          "request": {
            "url": "http://example.com/api/railguns/:identifier/zones",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "The zones that are currently using this Railgun"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "38d4f75e-b10c-4bb5-9b04-cc2276b949df"
            }
          ]
        },
        {
          "id": "0ddd3772-ecf1-4eeb-a5ec-f3b40d5df991",
          "name": "cloudflare-railgun-connections-for-a-zone-api",
          "request": {
            "url": "http://example.com/api/zones/:zone_identifier/railguns",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "A list of available Railguns the zone can use"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "a146f4c3-55a6-48de-ba9e-8732a94c1740"
            }
          ]
        },
        {
          "id": "6ae08ba2-b720-420d-a4fa-bdf92fdf303f",
          "name": "cloudflare-railgun-connections-for-a-zone-api1",
          "request": {
            "url": "http://example.com/api/zones/:zone_identifier/railguns/:identifier",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Details about a specific Railgun"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "a3de2a3d-482a-4eaa-9e9c-2819ccc26854"
            }
          ]
        },
        {
          "id": "76fe15f8-d44a-4964-ab60-aa66f62f896f",
          "name": "cloudflare-railgun-connections-for-a-zone-api",
          "request": {
            "url": "http://example.com/api/zones/:zone_identifier/railguns/:identifier?connected=%7B%7D",
            "method": "PATCH",
            "header": [
              {
                "key": "X-AUTH-EMAIL",
                "value": "{}",
                "description": "Email address associated with your account",
                "disabled": false
              },
              {
                "key": "X-AUTH-KEY",
                "value": "{}",
                "description": "API key generated on the My Account page",
                "disabled": false
              }
            ],
            "body": {
              "mode": "raw"
            },
            "description": "Connect or disconnect a Railgun"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "42424977-703a-4d51-a86c-7229e63c15bf"
            }
          ]
        },
        {
          "id": "cc8b748a-108e-4705-83c6-db013cc4f87d",
          "name": "cloudflare-railgun-connections-for-a-zone-api2",
          "request": {
            "url": "http://example.com/api/zones/:zone_identifier/railguns/:identifier/diagnose",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Test Railgun connection to the Zone"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "7320dee5-f8a4-46d4-b816-fee186ab7187"
            }
          ]
        }
      ]
    },
    {
      "name": "Users",
      "item": [
        {
          "id": "03effa55-2379-4057-88b7-b259d14d1186",
          "name": "cloudflare-user-api",
          "request": {
            "url": "http://example.com/api/user",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "User detailsn"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "6724bc92-9b60-40cf-b095-930cf5c226f4"
            }
          ]
        },
        {
          "id": "a796ba00-4827-4d4f-ab32-cc7b6e611251",
          "name": "cloudflare-user-api",
          "request": {
            "url": "http://example.com/api/user?country=%7B%7D&first_name=%7B%7D&last_name=%7B%7D&telephone=%7B%7D&zipcode=%7B%7D",
            "method": "PATCH",
            "header": [
              {
                "key": "X-AUTH-EMAIL",
                "value": "{}",
                "description": "Email address associated with your account",
                "disabled": false
              },
              {
                "key": "X-AUTH-KEY",
                "value": "{}",
                "description": "API key generated on the My Account page",
                "disabled": false
              }
            ],
            "body": {
              "mode": "raw"
            },
            "description": "Update part of your user details"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "84e4eba0-f255-4e24-bbae-8a3b0c6bc192"
            }
          ]
        }
      ]
    },
    {
      "name": "Billing History",
      "item": [
        {
          "id": "936800e0-a488-41c9-b081-4b67b5ca650e",
          "name": "cloudflare-user-billing-history-api",
          "request": {
            "url": "http://example.com/api/user/billing/history?action=%7B%7D&occured_at=%7B%7D&order=%7B%7D&page=%7B%7D&per_page=%7B%7D&type=%7B%7D",
            "method": "GET",
            "header": [
              {
                "key": "X-AUTH-EMAIL",
                "value": "{}",
                "description": "Email address associated with your account",
                "disabled": false
              },
              {
                "key": "X-AUTH-KEY",
                "value": "{}",
                "description": "API key generated on the My Account page",
                "disabled": false
              }
            ],
            "body": {
              "mode": "raw"
            },
            "description": "Access your billing history object"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "517064b7-82e7-4d94-a3be-ff9913391056"
            }
          ]
        }
      ]
    },
    {
      "name": "Billing Profile",
      "item": [
        {
          "id": "834af882-a12d-4f28-af56-b626f8be9b4a",
          "name": "cloudflare-user-billing-profile-api",
          "request": {
            "url": "http://example.com/api/user/billing/profile",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Access your billing profile object"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "e7d1ed9d-8b30-4c52-9ff6-7d4e8f24193f"
            }
          ]
        }
      ]
    },
    {
      "name": "User Level Firewall Access Rule",
      "item": [
        {
          "id": "1c52455b-7fc8-40da-89c2-a735aa7390cc",
          "name": "cloudflare-userlevel-firewall-access-rule-api",
          "request": {
            "url": "http://example.com/api/user/firewall/access_rules/rules?configuration_target=%7B%7D&configuration_value=%7B%7D&direction=%7B%7D&match=%7B%7D&mode=%7B%7D&order=%7B%7D&page=%7B%7D&per_page=%7B%7D",
            "method": "GET",
            "header": [
              {
                "key": "X-AUTH-EMAIL",
                "value": "{}",
                "description": "Email address associated with your account",
                "disabled": false
              },
              {
                "key": "X-AUTH-KEY",
                "value": "{}",
                "description": "API key generated on the My Account page",
                "disabled": false
              }
            ],
            "body": {
              "mode": "raw"
            },
            "description": "Search, sort, and filter IP/country access rules"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "8246607d-7e59-4c3b-9874-33610409cdc1"
            }
          ]
        },
        {
          "id": "16c14b60-b4e9-48f3-a71a-9416535947fd",
          "name": "cloudflare-userlevel-firewall-access-rule-api",
          "request": {
            "url": "http://example.com/api/user/firewall/access_rules/rules?configuration=%7B%7D&mode=%7B%7D&value=%7B%7D",
            "method": "POST",
            "header": [
              {
                "key": "X-AUTH-EMAIL",
                "value": "{}",
                "description": "Email address associated with your account",
                "disabled": false
              },
              {
                "key": "X-AUTH-KEY",
                "value": "{}",
                "description": "API key generated on the My Account page",
                "disabled": false
              }
            ],
            "body": {
              "mode": "raw"
            },
            "description": "Make a new IP, IP range, or country access rule for all zones owned by the user"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "50e6bfa4-170a-4165-9e31-81823ed3b41e"
            }
          ]
        },
        {
          "id": "50930027-1621-4108-834c-f94c28979707",
          "name": "cloudflare-userlevel-firewall-access-rule-api",
          "request": {
            "url": "http://example.com/api/user/firewall/access_rules/rules/:identifier",
            "method": "DELETE",
            "body": {
              "mode": "raw"
            },
            "description": "Remove an access rule so it is no longer evaluated during requests"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "5be03eff-4595-4093-84ea-865dd21b57c3"
            }
          ]
        },
        {
          "id": "8a5a142d-7d5b-46e1-be3c-de7805866026",
          "name": "cloudflare-userlevel-firewall-access-rule-api",
          "request": {
            "url": "http://example.com/api/user/firewall/access_rules/rules/:identifier?configuration=%7B%7D&mode=%7B%7D&value=%7B%7D",
            "method": "PATCH",
            "header": [
              {
                "key": "X-AUTH-EMAIL",
                "value": "{}",
                "description": "Email address associated with your account",
                "disabled": false
              },
              {
                "key": "X-AUTH-KEY",
                "value": "{}",
                "description": "API key generated on the My Account page",
                "disabled": false
              }
            ],
            "body": {
              "mode": "raw"
            },
            "description": "Update rule state and/or configuration"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "bc275964-c37e-472a-a172-e4dd110f986d"
            }
          ]
        }
      ]
    },
    {
      "name": "User Invites",
      "item": [
        {
          "id": "fc0646ff-86c5-4cc9-a5f2-17597b21c217",
          "name": "cloudflare-userx27s-invites-api",
          "request": {
            "url": "http://example.com/api/user/invites",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "List all invitations associated with my user"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "daf90908-2bf8-4ecb-b1b4-e2a43bab59d2"
            }
          ]
        },
        {
          "id": "4c40a4f8-cb64-4390-8457-0407ac24e5f6",
          "name": "cloudflare-userx27s-invites-api1",
          "request": {
            "url": "http://example.com/api/user/invites/:identifier",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Get the details of an invitation"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "86be0a6e-412c-49b8-bb5a-7c3f2570879f"
            }
          ]
        },
        {
          "id": "b79bbcc7-b8e8-4363-8cce-0c9fa121a84c",
          "name": "cloudflare-userx27s-invites-api",
          "request": {
            "url": "http://example.com/api/user/invites/:identifier?status=%7B%7D",
            "method": "PATCH",
            "header": [
              {
                "key": "X-AUTH-EMAIL",
                "value": "{}",
                "description": "Email address associated with your account",
                "disabled": false
              },
              {
                "key": "X-AUTH-KEY",
                "value": "{}",
                "description": "API key generated on the My Account page",
                "disabled": false
              }
            ],
            "body": {
              "mode": "raw"
            },
            "description": "Respond to an invitation"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "d9c63db0-2f2d-44f2-82d9-301b3a38f1d6"
            }
          ]
        }
      ]
    },
    {
      "name": "User Organizations",
      "item": [
        {
          "id": "52a3ebce-2c08-4262-9ec6-afab72133212",
          "name": "cloudflare-userx27s-organizations-api",
          "request": {
            "url": "http://example.com/api/user/organizations?direction=%7B%7D&match=%7B%7D&name=%7B%7D&order=%7B%7D&page=%7B%7D&per_page=%7B%7D&status=%7B%7D",
            "method": "GET",
            "header": [
              {
                "key": "X-AUTH-EMAIL",
                "value": "{}",
                "description": "Email address associated with your account",
                "disabled": false
              },
              {
                "key": "X-AUTH-KEY",
                "value": "{}",
                "description": "API key generated on the My Account page",
                "disabled": false
              }
            ],
            "body": {
              "mode": "raw"
            },
            "description": "List organizations the user is associated with"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "81ebf875-82f4-4cd4-845e-fd35154fefbf"
            }
          ]
        },
        {
          "id": "806c479e-d556-4afa-a652-01d3ce8d5c67",
          "name": "cloudflare-userx27s-organizations-api",
          "request": {
            "url": "http://example.com/api/user/organizations/:identifier",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Get a specific organization the user is associated with"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "5e721e9f-d758-4c90-a638-e91e53849e46"
            }
          ]
        },
        {
          "id": "18769a94-a130-458e-a18a-f82303739d18",
          "name": "cloudflare-userx27s-organizations-api",
          "request": {
            "url": "http://example.com/api/user/organizations/:identifier",
            "method": "DELETE",
            "body": {
              "mode": "raw"
            },
            "description": "Remove association to an organization"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "a749f627-204d-4697-9a61-20b1dae4397a"
            }
          ]
        }
      ]
    }
  ]
}