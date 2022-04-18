## AWS production access 

step 1: you can do it using aws cli just write these command 

```
aws sesv2 put-account-details \
--production-access-enabled \
--mail-type TRANSACTIONAL \
--website-url https://example.com \
--use-case-description "Use case description" \
--additional-contact-email-addresses info@example.com \
--contact-language EN

```

In the preceding command, do the following:

* Replace TRANSACTIONAL with the type of email that you plan to send through Amazon SES. You can specify either TRANSACTIONAL or PROMOTIONAL. If more than one value applies, specify the option that applies to the majority of the email that you plan to send.

* Replace https://example.com with the URL of your website. Providing this information helps us better understand the type of content that you plan to send.

* Replace Use case description with a description of how you plan to use Amazon SES to send email. To help us process your request, you should answer the following questions:

    * How do you plan to build or acquire your mailing list?

    * How do you plan to handle bounces and complaints?

    * How can recipients opt out of receiving email from you?

    * How did you choose the sending rate or sending quota that you specified in this request?

* Replace info@example.com with the email addresses where you want to receive communications about your account. This can be a comma-separated list of up to 4 email addresses.

* Replace EN with your preferred language. You can specify EN for English or JP for Japanese.

Once you submit a review of your account details, you can’t edit your details until the review is complete. The AWS Support team provides an initial response to your request within 24 hours.

In order to prevent our systems from being used to send unsolicited or malicious content, we have to consider each request carefully. If we're able to do so, we'll grant your request within this 24-hour period. However, if we need to obtain additional information from you, it might take longer to resolve your request. We might not be able to grant your request if your use case doesn't align with our policies.