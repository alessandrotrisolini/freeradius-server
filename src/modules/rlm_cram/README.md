# rlm_cram
## Metadata
<dl>
  <dt>category</dt><dd>authentication</dd>
</dl>

## Summary
Implements CRAM-MD5 authentication, a challenge response protocol similar to CHAP. CRAM is defined by RFC 2195.

## Detail
Status for this module is experemental. There is no publically available software to support CRAM authentication via
RADIUS yet.

CRAM mail authentication (APOP, CRAM-MD5)


Attributes used (Vendor Code/PEN: 11406, you may change it to your own) 101 (Sandy-Mail-Authtype), selects CRAM
protocol, possible values:

  - 2: CRAM-MD5
  - 3: APOP
  - 8: CRAM-MD4
  - 9: CRAM-SHA1

102 (Sandy-Mail-Challenge), contains server's challenge (usually text banner) 103 (Sandy-Mail-Response), contains
client's response, 16 octets for APOP/CRAM-MD5/CRAM-MD4, 20 octets for CRAM-SHA1.

See dictionary.sandy and Standard.draft for attribute descriptions.

