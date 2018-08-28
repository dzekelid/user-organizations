{
  "info": {
    "name": "CloudFlare Remove association to an organization",
    "_postman_id": "41f7fa24-ccc2-4f8d-bcd3-f87fb6dd89df",
    "description": "Remove association to an organization",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Subscriptions",
      "item": [
        {
          "id": "44eefc93-b57e-4e7f-9897-4bc576e6fd7f",
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
              "id": "638ef68f-02b4-4d79-81ad-73a5a9997014"
            }
          ]
        },
        {
          "id": "6e85bed1-7c02-4de2-b568-e08d2ed56441",
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
              "id": "1afab2ce-23c2-4c62-b37e-a080803b4f2b"
            }
          ]
        }
      ]
    },
    {
      "name": "Zones",
      "item": [
        {
          "id": "d465e6f8-a28a-4b7b-9c2e-b0dec7776a0f",
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
              "id": "9e600096-20a7-404a-a6d3-c1bfd930fcda"
            }
          ]
        },
        {
          "id": "3e9e1ac6-d7dc-4cb1-800e-27f840ff2a23",
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
              "id": "c2569650-10b9-47ad-b3d1-80465a50d84f"
            }
          ]
        },
        {
          "id": "73400b6e-8fb5-4131-8002-8bef5eca9371",
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
              "id": "b94f63ed-23d8-40a1-9d18-aa1bfac75942"
            }
          ]
        }
      ]
    },
    {
      "name": "Certificates",
      "item": [
        {
          "id": "d7a8804b-396f-44ab-8da2-da3ea44aa5e4",
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
              "id": "51a1f208-62cb-42d3-b783-a062d8b76805"
            }
          ]
        },
        {
          "id": "af2d8d34-2ac4-4d29-aa7b-4df0413d7bea",
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
              "id": "8f3fa213-ce40-42ea-8705-51e6d0b62e9e"
            }
          ]
        },
        {
          "id": "61e4f817-91e5-4029-9799-44a4cafd48a8",
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
              "id": "70f803ae-b6ee-412e-99a4-61da55545451"
            }
          ]
        },
        {
          "id": "a04b9dcf-a2c4-4bc5-bbc4-ffe9d3c81ad2",
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
              "id": "f98dc340-0372-44ab-be9a-ebec25fae591"
            }
          ]
        },
        {
          "id": "f98429ce-d486-45bd-ae89-33518b77d8af",
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
              "id": "d1719047-ffde-4175-8c7b-d59e6adefc4a"
            }
          ]
        },
        {
          "id": "2b0843a3-efdd-4c28-a6d0-523a9bff3679",
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
              "id": "9414197d-ad51-49e1-a6bd-99f1a8d53734"
            }
          ]
        }
      ]
    },
    {
      "name": "Records",
      "item": [
        {
          "id": "36af7795-c75e-4782-adf6-5796e0ec4bf3",
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
              "id": "50aa5606-98a8-4db6-baa9-ea0f9c04189b"
            }
          ]
        },
        {
          "id": "c82dece6-9429-4d8c-8a5e-c5d29056d9c0",
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
              "id": "e033654e-2ab5-44a4-80c5-0ab08d99087a"
            }
          ]
        },
        {
          "id": "c65da654-d537-4ab0-acbe-6c37b0a19a7a",
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
              "id": "37ef332b-8e54-49c1-84fd-1c18064b7777"
            }
          ]
        },
        {
          "id": "5eb38666-5466-439f-a504-261b554bc79f",
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
              "id": "0e29a80e-ce30-4fa4-8b20-027f4a6b5fc0"
            }
          ]
        },
        {
          "id": "40ec1076-9e56-4367-adb2-e2258393c1ad",
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
              "id": "631e3a6b-fdd5-4a2c-83d0-cb5aed021988"
            }
          ]
        }
      ]
    },
    {
      "name": "Firewall Access Rule",
      "item": [
        {
          "id": "70110d38-d9d1-4932-aa7f-19a14c6d30e2",
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
              "id": "02c5ae2f-b5a7-42e5-9292-cdd148635d0d"
            }
          ]
        },
        {
          "id": "e1b9e24d-b593-4a04-aa5f-6736ffda71bf",
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
              "id": "442e8a68-63b5-4827-b9c8-9dc349c4f953"
            }
          ]
        },
        {
          "id": "c7ed4f5d-7d8b-4d41-8ee9-b3d94435fb83",
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
              "id": "2e7fe21e-be1e-4bd3-8640-1433f2159dc8"
            }
          ]
        },
        {
          "id": "fa48e608-df59-4085-bdfa-188f5a8e172a",
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
              "id": "98170085-f79b-4497-b8a3-c9f604ca9972"
            }
          ]
        }
      ]
    },
    {
      "name": "Keyless Certificates",
      "item": [
        {
          "id": "8461bea3-2b4b-48c1-a341-46112830f4d0",
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
              "id": "94d0754a-8c0f-4174-836d-5c931b69e830"
            }
          ]
        },
        {
          "id": "9a0eed2b-c879-49da-8c6b-97c47c24c4db",
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
              "id": "e1e686a5-5e8f-42b0-ae65-748c187e29b9"
            }
          ]
        },
        {
          "id": "bd373c8d-0bd9-45c7-aa27-54225ddcccc9",
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
              "id": "247d6562-c286-427e-a805-e05ec76a4f6d"
            }
          ]
        },
        {
          "id": "b82ec245-7e98-42a8-8fec-5c273b664850",
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
              "id": "9749737e-ccc3-4df0-b059-351f874e73d7"
            }
          ]
        },
        {
          "id": "c0209af1-3e53-475c-ad1c-d438edb57ecd",
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
              "id": "2bd3e4a2-f8c6-463a-8b35-efd6c1b9c37f"
            }
          ]
        }
      ]
    },
    {
      "name": "Organization Invites",
      "item": [
        {
          "id": "35a3c84e-942a-4d79-8ade-6d9862193303",
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
              "id": "965a058e-d59b-419d-8270-5e858dd7f597"
            }
          ]
        },
        {
          "id": "c10980a8-b158-479c-b6ac-27c61d4de3d6",
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
              "id": "7fa0ce1c-5f32-4c05-8b3e-21ab4e7422d9"
            }
          ]
        },
        {
          "id": "5131a464-40fc-4e0a-bf3f-bd29811bb12d",
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
              "id": "5386fb22-e369-4843-b7fa-e6d1f763c977"
            }
          ]
        },
        {
          "id": "ff1ef3fb-7df9-40c7-88bc-6238f70ac0da",
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
              "id": "5cb45a4d-9847-47d7-986f-5b283ac44bdd"
            }
          ]
        },
        {
          "id": "c6fdc925-7109-45ce-a815-2b5de7bb3d8c",
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
              "id": "ca2c00cd-4ac3-4e31-9171-69b06feb8503"
            }
          ]
        }
      ]
    },
    {
      "name": "Organization Members",
      "item": [
        {
          "id": "5d4dac35-5ea1-44ab-a02f-bda7c4cd8ef7",
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
              "id": "9d57c98c-212d-4c8b-9154-0c70c01ef4b3"
            }
          ]
        },
        {
          "id": "8e85b887-765b-46a8-8040-08c7036bcf3d",
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
              "id": "0d7d2f93-bb58-4b16-b5b4-d23633c9f5e6"
            }
          ]
        },
        {
          "id": "f2bca585-4ccc-4e32-bcae-230073b2a011",
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
              "id": "8ee6d83d-fe0d-4e8c-8f0b-b5ae3610d4ae"
            }
          ]
        },
        {
          "id": "450c81c4-cd6f-480a-ac98-b8ec3d4146a0",
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
              "id": "9240e69b-473f-4895-a44d-ff1d9c36bb25"
            }
          ]
        }
      ]
    },
    {
      "name": "Organization Roles",
      "item": [
        {
          "id": "573b9ebd-15cf-4afe-abbc-702ae1e54459",
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
              "id": "11771280-7ec1-4fc2-a675-32f87962e2c5"
            }
          ]
        },
        {
          "id": "9ba76d36-6419-4cc0-98be-5a3d2f465861",
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
              "id": "a5318bb6-109a-4514-8d76-8a9bbaabf88c"
            }
          ]
        }
      ]
    },
    {
      "name": "Organization Firewall Access Rules",
      "item": [
        {
          "id": "a93101ce-cfd4-4791-890a-72b5f1a755c0",
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
              "id": "7332ff36-cd81-4028-8637-95a06c32c72d"
            }
          ]
        },
        {
          "id": "b59774b2-00d5-43c5-961b-635240b5ad9a",
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
              "id": "d044a6d7-2f20-4430-beb9-0b97f1e8929d"
            }
          ]
        },
        {
          "id": "6fe69f98-c163-43a9-b34d-0553e0d8fbab",
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
              "id": "2c6d29cd-a0c0-4018-8815-39611cc072bb"
            }
          ]
        },
        {
          "id": "d82e90d8-5562-4d05-8ff9-50a8df07c985",
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
              "id": "6fe880f0-52fb-4d87-b12f-15d413045e25"
            }
          ]
        }
      ]
    },
    {
      "name": "Organizations",
      "item": [
        {
          "id": "bb858bdd-d99d-4643-b724-3b4d6831adcd",
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
              "id": "f2f0fbb4-d05b-4d2f-bde2-9db7f9088fe7"
            }
          ]
        },
        {
          "id": "6ef1e517-323c-405c-9c04-1f152150e382",
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
              "id": "1f9f35e8-b534-47f3-b237-0615135c28dd"
            }
          ]
        }
      ]
    },
    {
      "name": "Performance",
      "item": [
        {
          "id": "d7a1022a-4595-42e9-87a3-0038ffd2308c",
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
              "id": "57d4583d-5f61-45b2-93f8-7cc232fe21fa"
            }
          ]
        },
        {
          "id": "15648421-6666-4f4d-9b73-9e2702bf8f6f",
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
              "id": "b48496a2-c1a5-4215-841b-84da788a3ddd"
            }
          ]
        },
        {
          "id": "7cabdac2-bc80-4885-99e9-320292e6cee8",
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
              "id": "560e12ab-18e7-4828-a1d5-04c8dfb6538f"
            }
          ]
        },
        {
          "id": "34c18e7f-bae3-4f9a-9493-cd3a807d75ab",
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
              "id": "8cf53531-46d6-4828-95af-443cf3d8d50f"
            }
          ]
        },
        {
          "id": "2eac3049-4f5e-4594-8254-6035fe71a4be",
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
              "id": "cb1bdf5e-690b-4699-a548-235d5145d3f6"
            }
          ]
        },
        {
          "id": "cede4725-bc1f-43cf-a17c-6f11deb70399",
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
              "id": "0964771a-24da-4bd2-b4cb-d41cd375970c"
            }
          ]
        },
        {
          "id": "41f00e7b-be9d-4562-9e5b-336e4573a004",
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
              "id": "001b0f34-1ad2-4304-9b6d-578602b46fd1"
            }
          ]
        },
        {
          "id": "de197f95-9b4a-4af9-8baf-bdab98cac756",
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
              "id": "52231685-9bfc-4bb4-9c9e-dbc7c8803462"
            }
          ]
        },
        {
          "id": "f0830f71-34b4-48f9-9a61-35bb9183d2c0",
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
              "id": "e9e5bc26-3820-4eba-81bd-0ad4a2fa13d3"
            }
          ]
        },
        {
          "id": "ea927219-719f-41a7-85d9-e236ffbe00ed",
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
              "id": "05c8876f-a8ad-4dbb-8e44-b85f79dc4227"
            }
          ]
        }
      ]
    },
    {
      "name": "Users",
      "item": [
        {
          "id": "1cb17aa7-2d2d-4fa8-82b9-939fee7b8d03",
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
              "id": "e28e1520-570a-4174-9619-148463cb828f"
            }
          ]
        },
        {
          "id": "39551227-ea34-4759-9e23-66bcd7540889",
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
              "id": "d766026e-50b2-4735-8fda-7f702b902522"
            }
          ]
        }
      ]
    },
    {
      "name": "Billing History",
      "item": [
        {
          "id": "b2efcccb-24f6-459e-bcfb-614393e0798d",
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
              "id": "edbf995a-8859-42ec-b040-533f1ab449ef"
            }
          ]
        }
      ]
    },
    {
      "name": "Billing Profile",
      "item": [
        {
          "id": "be930a76-4f0a-4184-8489-6e811db5fe21",
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
              "id": "393d462c-1c8c-48d6-afe0-56a3732bb5ce"
            }
          ]
        }
      ]
    },
    {
      "name": "User Level Firewall Access Rule",
      "item": [
        {
          "id": "983a1d36-bf45-4338-ab24-1223e059b32b",
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
              "id": "93b3bf67-3c0f-411a-8e8c-c6903cf80d77"
            }
          ]
        },
        {
          "id": "1dbcee93-00c9-49fe-9f94-a60c47e70b0f",
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
              "id": "6b511743-4de4-486e-942e-8a31f5698937"
            }
          ]
        },
        {
          "id": "f15fb3e0-f4be-48d8-8804-0bbeae1f766d",
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
              "id": "d591ebe1-09da-4b2c-8a8a-9054585d304c"
            }
          ]
        },
        {
          "id": "181dcf8a-9f91-41e0-9a12-d7eac0444840",
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
              "id": "e5009e0f-811b-4381-a969-4789afbdf91b"
            }
          ]
        }
      ]
    },
    {
      "name": "User Invites",
      "item": [
        {
          "id": "28ac548c-5c31-46af-b3a1-15f9088ef890",
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
              "id": "e89463b1-7ab3-42e3-887c-a352c271e788"
            }
          ]
        },
        {
          "id": "00a8d971-8a8a-4182-aa4b-958b2ef90286",
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
              "id": "e12c7915-be6c-4beb-955e-1b7981d74588"
            }
          ]
        },
        {
          "id": "b882cd10-a5d7-4a36-8a4d-5203a241b340",
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
              "id": "d1f67c88-937a-435a-a645-0b366a82e7d3"
            }
          ]
        }
      ]
    },
    {
      "name": "User Organizations",
      "item": [
        {
          "id": "67ce48e5-ffc0-4cf0-a6f0-05f25c7259c8",
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
              "id": "b031eb43-ad15-4407-8483-51c26c28b9d4"
            }
          ]
        },
        {
          "id": "d36048f9-0de2-4894-8713-6a5da0773d80",
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
              "id": "23c717a2-e206-45a4-b56b-10404df55742"
            }
          ]
        }
      ]
    }
  ]
}