<!DOCTYPE html>
<html>
<head>
    <title>App Redirect</title>
    <script>
        window.onload = function() {
            var userAgent = navigator.userAgent || navigator.vendor || window.opera;

            // Redirect based on user agent
            if (/android/i.test(userAgent)) {
                window.location.href = "https://play.google.com/store/apps/details?id=com.prasarana.pulse.v4";
            } else if (/iPad|iPhone|iPod/.test(userAgent) && !window.MSStream) {
                window.location.href = "https://apps.apple.com/us/app/myrapid-pulse/id6736607730";
            } else {
                // Redirect to the specified URL for non-mobile devices
                window.location.href = "https://myrapid.com.my/pulse/mobile-app/";
            }
        }
    </script>
</head>
<body>
</body>
</html>
