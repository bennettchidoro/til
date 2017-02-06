# Rails Console Sandbox Mode

Rails gives us the option to start the console in sandbox mode. When we enter the console in sandbox mode any database operations we make are automatically "rolled back" when we exit the console.

Start the rails console in sandbox mode with: `$ rails c --sandbox`

![](https://s3.amazonaws.com/til-stuff/tty.gif?X-Amz-Date=20170206T034741Z&X-Amz-Expires=300&X-Amz-Algorithm=AWS4-HMAC-SHA256&X-Amz-Signature=2b4f24d3a71c303260d0bd7956d187567ca9dbd9f5d59362c9bf1d25428ecba9&X-Amz-Credential=ASIAIFMOWLPN2CEWH2CQ/20170206/us-east-1/s3/aws4_request&X-Amz-SignedHeaders=Host&x-amz-security-token=FQoDYXdzECUaDCaq5u6s50VCeUysfiL6Ad/vMeGvYGaUPIkV6lWNZJ52ZcTWAJI7Bn0TIrtMr4J6hdF9718Cgqr3tIX24ZlqB7fYpIbGVIz80OwVreKtCbxfvUNVcnyxvs/FXbbt/2yiLCynR6qLCGyxu0TTNQ/tqbU5ZxHBHo85Ndq7aB5OFfE64MwzMvZcU%2BWLPAC1CNG6jsgDfKWqEmyq0IWSrMueOBcNMsGJ5u3hBVPSBJdervOZg3Nwm/geWOh/U7k8ZMcadMEBSlJCjmF9D1mW5O1CsAZTbSLVePl0abfX%2BethmQeWSy1fTFAlDTHbIHTCfYfytkElzsTQi8vnEPq25A88LdyPTuVlMrUF/0UoxuPfxAU%3D)

Sandbox mode comes in handy when we want to experiment with the database without permanently changing our data.
