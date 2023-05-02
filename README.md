# SimpleImport
Just getting started


<!DOCTYPE html>
<html>

<head>
    <script>
        const fireConsentChangedEvent = () => {
            const event = new Event('onetrustConsentChanged');
            window.dispatchEvent(event);
        }
    </script>

        <!-- OneTrust Cookies Consent Notice start for rec.net -->
        <script src="https://cdn.cookielaw.org/scripttemplates/otSDKStub.js" type="text/javascript" charset="UTF-8"
        data-domain-script="9cb9be76-5401-4e9c-b86f-45e7daeb55e0"></script>
        <script type="text/javascript">
            function OptanonWrapper() { fireConsentChangedEvent(); }
        </script>
        <!-- OneTrust Cookies Consent Notice end for rec.net -->

    <!-- Google Tag Manager -->
    <script>
        (function (w, d, s, l, i) {
            w[l] = w[l] || []; w[l].push({
                'gtm.start':
                    new Date().getTime(), event: 'gtm.js'
            }); var f = d.getElementsByTagName(s)[0],
                j = d.createElement(s), dl = l != 'dataLayer' ? '&l=' + l : ''; j.async = true; j.src =
                    'https://www.googletagmanager.com/gtm.js?id=' + i + dl; f.parentNode.insertBefore(j, f);
        })(window, document, 'script', 'dataLayer', 'GTM-5SVMRSR');
    </script>
    <!-- End Google Tag Manager -->
    <script>
        // Inline code from https://unpkg.com/web-vitals/dist/polyfill.js
        // Kicks off the web vitals measurement process
        !function () { var e, t, n, i, r = { passive: !0, capture: !0 }, a = new Date, o = function () { i = [], t = -1, e = null, f(addEventListener) }, c = function (i, r) { e || (e = r, t = i, n = new Date, f(removeEventListener), u()) }, u = function () { if (t >= 0 && t < n - a) { var r = { entryType: "first-input", name: e.type, target: e.target, cancelable: e.cancelable, startTime: e.timeStamp, processingStart: e.timeStamp + t }; i.forEach((function (e) { e(r) })), i = [] } }, s = function (e) { if (e.cancelable) { var t = (e.timeStamp > 1e12 ? new Date : performance.now()) - e.timeStamp; "pointerdown" == e.type ? function (e, t) { var n = function () { c(e, t), a() }, i = function () { a() }, a = function () { removeEventListener("pointerup", n, r), removeEventListener("pointercancel", i, r) }; addEventListener("pointerup", n, r), addEventListener("pointercancel", i, r) }(t, e) : c(t, e) } }, f = function (e) { ["mousedown", "keydown", "touchstart", "pointerdown"].forEach((function (t) { return e(t, s, r) })) }, p = "hidden" === document.visibilityState ? 0 : 1 / 0; addEventListener("visibilitychange", (function e(t) { "hidden" === document.visibilityState && (p = t.timeStamp, removeEventListener("visibilitychange", e, !0)) }), !0); o(), self.webVitals = { firstInputPolyfill: function (e) { i.push(e), u() }, resetFirstInputPolyfill: o, get firstHiddenTime() { return p } } }();
    </script>
    <meta charset="utf-8" />
    <meta name="description"
        content="Rec Room is the best place to build and play games together. Chat, hang out, explore MILLIONS of rooms, or build something new to share with us all!" />
    <meta name="keywords" content="Social,VR,Game,Free" />
    <meta name="viewport" content="width=device-width, initial-scale=1.0" />
    

<meta property="og:type" content="website" />
<meta property="og:url" content="https://rec.net/user/Keima" />
<meta property="og:title" content="@Keima" />
<meta property="og:description" content="Rec Room is the best place to build and play games together. Chat, hang out, explore MILLIONS of rooms, or build something new to share with us all!" />
<meta property="og:image" content="https://img.rec.net/DefaultProfileImage" />
<meta name="apple-itunes-app" content="app-id=1450306065, app-argument=https://rec.net/user/Keima" />

<meta name="twitter:card" content="summary_large_image" />


    <title>RecNet</title>
    <base href="/" />

    <link rel="stylesheet" href="https://fonts.googleapis.com/css?family=Nunito:800">
    <link rel="stylesheet" href="https://fonts.googleapis.com/css?family=Roboto:100,200,300,400,500,600,700">
    <link rel="stylesheet" href="https://fonts.googleapis.com/css?family=Roboto+Slab:100,200,300,400,500,600,700">
    <link rel="stylesheet" href="https://fonts.googleapis.com/icon?family=Material+Icons">
    <link rel="stylesheet" href="/dist/site.css" />

    <script src="https://cdnjs.cloudflare.com/ajax/libs/es6-promise/4.1.1/es6-promise.auto.min.js"
        integrity="sha384-kM3+BR0fKGmv8mDasMGLSHdqcbgWHUNWV1rAL+tkqnH578xS82vhlu9gR5BHhBai"
        crossorigin="anonymous"></script>

    <script>

        if (typeof Object.assign !== 'function') {
            // Must be writable: true, enumerable: false, configurable: true
            Object.defineProperty(Object, "assign", {
                value: function assign(target, varArgs) { // .length of function is 2
                    'use strict';
                    if (target === null) { // TypeError if undefined or null
                        throw new TypeError('Cannot convert undefined or null to object');
                    }

                    var to = Object(target);

                    for (var index = 1; index < arguments.length; index++) {
                        var nextSource = arguments[index];

                        if (nextSource !== null) { // Skip over if undefined or null
                            for (var nextKey in nextSource) {
                                // Avoid bugs when hasOwnProperty is shadowed
                                if (Object.prototype.hasOwnProperty.call(nextSource, nextKey)) {
                                    to[nextKey] = nextSource[nextKey];
                                }
                            }
                        }
                    }
                    return to;
                },
                writable: true,
                configurable: true
            });
        }

        // Production steps of ECMA-262, Edition 6, 22.1.2.1
        if (!Array.from) {
            Array.from = (function () {
                var toStr = Object.prototype.toString;
                var isCallable = function (fn) {
                    return typeof fn === 'function' || toStr.call(fn) === '[object Function]';
                };
                var toInteger = function (value) {
                    var number = Number(value);
                    if (isNaN(number)) { return 0; }
                    if (number === 0 || !isFinite(number)) { return number; }
                    return (number > 0 ? 1 : -1) * Math.floor(Math.abs(number));
                };
                var maxSafeInteger = Math.pow(2, 53) - 1;
                var toLength = function (value) {
                    var len = toInteger(value);
                    return Math.min(Math.max(len, 0), maxSafeInteger);
                };

                // The length property of the from method is 1.
                return function from(arrayLike/*, mapFn, thisArg */) {
                    // 1. Let C be the this value.
                    var C = this;

                    // 2. Let items be ToObject(arrayLike).
                    var items = Object(arrayLike);

                    // 3. ReturnIfAbrupt(items).
                    if (arrayLike === null) {
                        throw new TypeError('Array.from requires an array-like object - not null or undefined');
                    }

                    // 4. If mapfn is undefined, then let mapping be false.
                    var mapFn = arguments.length > 1 ? arguments[1] : void undefined;
                    var T;
                    if (typeof mapFn !== 'undefined') {
                        // 5. else
                        // 5. a If IsCallable(mapfn) is false, throw a TypeError exception.
                        if (!isCallable(mapFn)) {
                            throw new TypeError('Array.from: when provided, the second argument must be a function');
                        }

                        // 5. b. If thisArg was supplied, let T be thisArg; else let T be undefined.
                        if (arguments.length > 2) {
                            T = arguments[2];
                        }
                    }

                    // 10. Let lenValue be Get(items, "length").
                    // 11. Let len be ToLength(lenValue).
                    var len = toLength(items.length);

                    // 13. If IsConstructor(C) is true, then
                    // 13. a. Let A be the result of calling the [[Construct]] internal method
                    // of C with an argument list containing the single item len.
                    // 14. a. Else, Let A be ArrayCreate(len).
                    var A = isCallable(C) ? Object(new C(len)) : new Array(len);

                    // 16. Let k be 0.
                    var k = 0;
                    // 17. Repeat, while k < len… (also steps a - h)
                    var kValue;
                    while (k < len) {
                        kValue = items[k];
                        if (mapFn) {
                            A[k] = typeof T === 'undefined' ? mapFn(kValue, k) : mapFn.call(T, kValue, k);
                        } else {
                            A[k] = kValue;
                        }
                        k += 1;
                    }
                    // 18. Let putStatus be Put(A, "length", len, true).
                    A.length = len;
                    // 20. Return A.
                    return A;
                };
            }());
        }

    </script>

    <style>
        html,
        body,
        #react-app {
            width: 100%;
            height: 100%;
            padding: 0;
            margin: 0;
            font-family: "Roboto" -apple-system BlinkMacSystemFont "Segoe UI""Helvetica Neue" Arial sans-serif "Apple Color Emoji""Segoe UI Emoji""Segoe UI Symbol";
        }

        body {
            overflow: hidden;
        }

        b {
            font-weight: 500
        }

        button:focus {
            outline: none
        }

        ::-webkit-scrollbar {
            height: 8px;
            width: 8px;
        }

        ::-webkit-scrollbar-track {
            background-color: rgba(0, 0, 0, 0.05);
        }

        ::-webkit-scrollbar-thumb {
            background-color: #f16e46;
            /*rgba(0, 0, 0, 0.05);*/
            -webkit-box-shadow: inset 0 0 6px rgba(0, 0, 0, 0.5);
        }

        ::-webkit-scrollbar-corner {
            background: rgba(0, 0, 0, 0.05);
        }

        * {
            -webkit-overflow-scrolling: touch;
        }

        /*
            These pagination styles are copied from bootstrap.css. We don't include the entire bootstrap.css
            because it applies globally and messes up our existing styles .
        */
        .pagination {
            display: -ms-flexbox;
            display: flex;
            padding-left: 0;
            list-style: none;
            border-radius: 0.25rem;
        }

        .page-link {
            position: relative;
            display: block;
            padding: 0.5rem 0.75rem;
            margin-left: -1px;
            line-height: 1.25;
            color: #007bff;
            background-color: #fff;
            border: 1px solid #dee2e6;
        }

        .page-link:hover {
            z-index: 2;
            color: #0056b3;
            text-decoration: none;
            background-color: #e9ecef;
            border-color: #dee2e6;
        }

        .page-link:focus {
            z-index: 2;
            outline: 0;
            box-shadow: 0 0 0 0.2rem rgba(0, 123, 255, 0.25);
        }

        .page-link:not(:disabled):not(.disabled) {
            cursor: pointer;
        }

        .page-item:first-child .page-link {
            margin-left: 0;
            border-top-left-radius: 0.25rem;
            border-bottom-left-radius: 0.25rem;
        }

        .page-item:last-child .page-link {
            border-top-right-radius: 0.25rem;
            border-bottom-right-radius: 0.25rem;
        }

        .page-item.active .page-link {
            z-index: 1;
            color: #fff;
            background-color: #007bff;
            border-color: #007bff;
        }

        .page-item.disabled .page-link {
            color: #6c757d;
            pointer-events: none;
            cursor: auto;
            background-color: #fff;
            border-color: #dee2e6;
        }

        .pagination-lg .page-link {
            padding: 0.75rem 1.5rem;
            font-size: 1.25rem;
            line-height: 1.5;
        }

        .pagination-lg .page-item:first-child .page-link {
            border-top-left-radius: 0.3rem;
            border-bottom-left-radius: 0.3rem;
        }

        .pagination-lg .page-item:last-child .page-link {
            border-top-right-radius: 0.3rem;
            border-bottom-right-radius: 0.3rem;
        }

        .pagination-sm .page-link {
            padding: 0.25rem 0.5rem;
            font-size: 0.875rem;
            line-height: 1.5;
        }

        .pagination-sm .page-item:first-child .page-link {
            border-top-left-radius: 0.2rem;
            border-bottom-left-radius: 0.2rem;
        }

        .pagination-sm .page-item:last-child .page-link {
            border-top-right-radius: 0.2rem;
            border-bottom-right-radius: 0.2rem;
        }

        @keyframes cheer {
            0% {
                opacity: 0.0;
                transform: scale(1.0, 1.0);
            }

            20% {
                opacity: 1.0;
                transform: scale(1.5, 1.5);
            }

            50% {
                transform: scale(1.0, 1.0);
            }

            80% {
                opacity: 1.0;
            }

            100% {
                opacity: 0.0;
            }
        }

        @font-face {
            font-family: 'Jost';
            src: url('https://cdn.rec.net/static/fonts/Jost-500-Medium.ttf') format('truetype'), url('https://cdn.rec.net/static/fonts/Jost-500-Medium.otf') format('opentype');
        }

        @font-face {
            font-family: 'NotoSans';
            src: url('https://cdn.rec.net/static/fonts/NotoSans-500-Medium.ttf') format('truetype');
        }

        @font-face {
            font-family: 'Bungee';
            src: url('https://cdn.rec.net/static/fonts/Bungee-Regular.ttf') format('truetype');
        }

        .ReactCollapse--collapse {
            transition: height 500ms;
        }

        /* Classes for sweetalert2 popup*/
        .alertPopup {
            padding: 0 !important;
            border-radius: 10px !important;
            justify-content: flex-start !important;
        }

        .alertHeader {
            width: 100% !important;
            padding: 0 !important;
        }

        .alertCloseButton {
            color: #757575 !important;
            width: 24px !important;
            height: 24px !important;
            padding-left: 0.25px !important;
            border-radius: 50% !important;
            background-color: rgba(255, 255, 255, 0.85) !important;
        }
    </style>


	<meta name="theme-color" content="#F16E46" />
	<link rel="manifest" href="/manifest.webmanifest" />
</head>

<body>

    


<!-- Google Tag Manager (noscript) -->
<noscript><iframe src="https://www.googletagmanager.com/ns.html?id=GTM-5SVMRSR" height="0" width="0"
        style="display:none;visibility:hidden"></iframe></noscript>
<!-- End Google Tag Manager (noscript) -->


<div id="react-app"></div>




    <script src="/dist/vendor.js?v=OtNSxCFfliClv6Q1ViLAKV9kZw-HkzpPXfLopjfkH8k"></script>

    
<!--https://sweetalert2.github.io/v7.html-->
<link rel="stylesheet" type="text/css" href="https://cdn.jsdelivr.net/sweetalert2/latest/sweetalert2.min.css">
<style>
    .swal2-container {
        z-index: 10000;
    }
</style>
<script>
    // See https://github.com/facebook/react/issues/20829#issuecomment-802088260
    if (!crossOriginIsolated) SharedArrayBuffer = ArrayBuffer;
</script>
<script>
    window.Config = {"serverUrls":{"Auth":"https://auth.rec.net","API":"https://api.rec.net","Accounts":"https://accounts.rec.net","Commerce":"https://commerce.rec.net","Data":"https://data.rec.net","Econ":"https://econ.rec.net","Matchmaking":"https://match.rec.net","Notifications":"https://notify.rec.net","Images":"https://img.rec.net","Chat":"https://chat.rec.net","Link":"https://link.rec.net","Clubs":"https://clubs.rec.net","Rooms":"https://rooms.rec.net","Website":"https://rec.net"},"amplitudeKey":"e1693a1003671058b6abc356c8ba8d59","stripePublishableKey":"pk_live_aWstgjERKMMvKtjPapYHJ8lY00OeqlhBMb","rudderStackKey":"24I1wL5g9rHCyiEa54cxIZW1gnr","reCaptchaKey":"6LcdbDwhAAAAAAd4lHqk9Tbx68BgqJZ_QoLtlD6n","appInsightsKey":null,"isDevEnv":false,"isTestEnv":false,"isProdEnv":true};
</script>
<script src="/dist/main-client.js?v=YCdgf8Uc6ba2lUrU0bdfLNeVMxqwOfjf14giAT6Mv8Q"></script>
<!--Snapchat share button-->
<!--https://snapkit.com/docs/creative-kit-web-->
<!--See Sharing.tsx for more info-->
<script src="https://sdk.snapkit.com/js/v1/create.js"></script>
<script>
    window.snapKitInitAndRenderSocialButtons = function () {
        var shareButtons = document.getElementsByClassName('snapchat-creative-kit-share');
        snap.creativekit.initalizeShareButtons(
            shareButtons
        );
        snap.creativekit.renderShareButtons();
    };
</script>




	<script>'serviceWorker'in navigator&&navigator.serviceWorker.register('/serviceworker', { scope: '/' })</script></body>

</html>
