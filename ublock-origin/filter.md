# Ublock Origin filters

## Features

- Removed youtube shorts.
- Blocks `.mov` and `.zip` TLDs from being loaded.
- Swedish filter.

### All filters

```
! Title: Frellwit's Swedish Filter
! Last updated: Tue, 16 Jul 2024 07:57:28 +0000
! Expires: 5 days
! Diff-Path: patches/2024.7.16.477.patch#swefilter
! Diff-Expires: 24 hours
! Description: A filter for uBlock Origin that aims to remove regional Swedish ads, tracking, annoyances, scams + badware, and unnecessary bloat.
! Homepage: https://github.com/lassekongo83/Frellwits-filter-lists
! License: https://github.com/lassekongo83/Frellwits-filter-lists/blob/master/LICENSE
! *** swefilter:Frellwits-Swedish-Filter.txt ***
.ads-gdprlock
.ax/ad/
.ax/images/banners/
.com/annonsmaterial/
.com/annons.$script,subdocument
.com/misc/loada.js
.html$subdocument,domain=flygtorget.se
.js?cb$domain=hemmanytt.se
.js?gcb$domain=hemmanytt.se
.nu/annons/
.nu/banner/
.nu/files/banner/
.nu/gfx/banner/
.nu/prebid$script
.php?annonsid=$image
.se/AdPlugins/
.se/Banners/
.se/Logger?
.se/Media/Banners/
.se/Static/banners/
.se/adson/$subdocument
.se/adstart.php
.se/advertisement_script
.se/advert$subdocument
.se/adx.js
.se/ad-delivery/
.se/ad/AdSpaceBlock/
.se/annons.$script,subdocument
.se/annons/$domain=~blocket.se
.se/assets/scripts/prebid
.se/banner.stat?
.se/banner/
.se/bildbank/banners/
.se/bilder/banners/
.se/blogcounter/image?
.se/common/js/tracking/
.se/counter/
.se/custom/ad/
.se/fightodds.plugin/fightodds.plugin.$script
.se/files/ads/$image
.se/files/annons/$image
.se/getBannerImage
.se/globalassets/banners/
.se/images/banners/
.se/images/banner/
.se/img/banners/
.se/js/ga.js|
.se/load-ads/
.se/logger.
.se/log/?
.se/makebnr.asp?
.se/misc/loada.js
.se/native?noBurtProfiles
.se/nonsec/banner/
.se/portalen-stats/register-view
.se/prebid$script
.se/pres/bnrs/$image
.se/revive/www/
.se/scripts/google-funding-choices.js
.se/sponsored/$image
.se/track/t.php?
.se/uploads/banners/
.se/uploads/images/banners/
.se/upload/annons/
.se/upload/_ads/
.se/wdg/tracking
.se/wdg/vda-active
.se/wp-content/banners/
.se/wp-content/uploads/_banners/
.se/xhr/add-impression/
.se/*/gillkom?$xmlhttprequest
.se/*/nativeadvertising/
.se/*/postkoll?$xmlhttprequest
.se/_Banners/
7an.se##.field--name-field-ad-banner-image
8sidor.se###cookie-banner
56kilo.se##.code-block:has(.shop-page-wp-grid)
56kilo.se##.featured-area, .awac-wrapper
56kilo.se##.penci-single-block[data-current-url*="cbd"]:has(a[href*="?ref="])
99.teknikveckan.se##.carousel-item-link:has-text(Annons:)
99.teknikveckan.se##.page-gutter.left, .page-gutter.right, [id^="bbPrisjakt"]
180.se##[class*="top-ad-"]
2000tv.se###bannerbox
Mobile-banner$image,domain=bokadirekt.se
accentmagasin.se##+js(nostif, n.modal)
adecco.se,ica.se,apotekhjartat.se,tele2.se###onetrust-consent-sdk
advokaten.se##.cookieconsent-optin-marketing
affarerinorr.se##a[href^="/nyheter/native-artiklar/"]
affarsstaden.se##+js(acs, jQuery, adblockdetect)
affarsvarlden.se##.article-tag-header:has-text(/Annons/i):upward(article)
affarsvarlden.se##.cookies-wrap, .Modal, .article-list-item--native, .advert-notice-box, .native-popup, .takeover-wrap, .native-notice-box, .darwin--content
aftonbladet.se##article[class^="article-wrapper"] ~ div:has-text(ANNONS)
aftonbladet.se##aside > div:has(h2:has-text(/^annons/i))
aftonbladet.se##a:has-text(Kommersiell text, innehåller annonslänkar)
aftonbladet.se##a[href^="https://kampanj."]:upward(1):not(section):not(div[class^="article-wrapper"])
aftonbladet.se##div[class^="css-"]:has([data-ad-subtype="mega"])
aftonbladet.se##main > section > div:first-child:matches-css(box-shadow: rgba(0, 0, 0, 0.2) 0px 0px 24px 0px)
aftonbladet.se##main > section > div[class^="css-"]:first-child:has(img[src*="closeButton"])
aftonbladet.se##p:has-text(/^PRESENTERAS AV$/):upward(1)
aftonbladet.se##section > div:has(h2:has-text(/^annons/i))
aftonbladet.se##span:has-text(/^annons/i):upward(a)
aftonbladet.se##strong:has-text(/ANNONS/i):upward(p)
aftonbladet.se###main > div > div > div:has(h2:has-text(/^annons/i))
aftonbladet.se###megaAd-placeholder, #superright-side, a[href*="/casinoguide"], [id^="adPlacement"], a[href^="https://kampanj.aftonbladet"], a[href*="/rabattkod"][data-test-tag="internal-link"], a[href^="/sportbladet/speltips/"], a[href*="aftonbladet.se/kampanj/"]
aftonbladet.se##:matches-path(/^/$/) p:has-text(Artikeln innehåller annonslänkar):upward(a)
aftonbladet.se##[data-ad-subtype]:upward(1):matches-css(min-height:/[0-9]+/)
aftonbladet.se,godare.se,livsstil.se##div[data-test-tag="prisjakt-carousel"], a[href^="/brandstudio"], div[class^="advertory-"]:not(.advertory-header-anchor)
aftonbladet.se,godare.se,livsstil.se,skonhetsredaktorerna.se,omni.se,omniekonomi.se,svd.se##.sp-message-open body:style(overflow:initial!important; position:unset!important; margin-top:unset!important;)
aftonbladet.se,halsasverige.se,mandarinmedia.se,nojesmagasinet.nu,stoppapressarna.se,langd.se,pressbladet.se,svenskpress.se,foretagsbladet.se,gestrikemagasinet.se,cfanytt.se,lasarnas.se,hembostad.nu,sportidrott.se,skolvarlden.se,computersweden.se,thatsup.se,arbetaren.se,sjofartstidningen.se##.advert
aftonbladet.se,livsstil.se,godare.se,byggahus.se,expressen.se,elle.se,femina.se,svenskdam.se,galamagasin.se,rodeo.net,familjeliv.se,vitaestilo.se##+js(href-sanitizer, a[href*="/t?a="], ?url)
aftonbladet.se,skonhetsredaktorerna.se##.ab_responsive_ads
agriaffaires.se,truckscorner.se,machineryzone.se##.dp--mb
aikfotboll.se,vaken.se,tidningen.djurskyddet.se##.banners
aikhockey.se,almtuna.com,bikkarlskoga.se,bjorkloven.com,brynas.se,difhockey.se,frolundahockey.com,farjestadbk.se,hockeyallsvenskan.se,hv71.se,ikoskarshamn.se,kalmarhockey.com,leksandsif.se,lhc.eu,luleahockey.se,malmoredhawks.com,modohockey.se,moraik.se,nybrovikings.com,orebrohockey.se,roglebk.se,shl.se,skellefteaaik.se,sodertaljesk.se,taif.nu,timraik.se,vaxjolakers.se,vikhockey.se,vik.se,ostersundik.com##a[href*="svenskaspel.se"][target]
aip.nu##[class*="feed-ad"]
aip.nu,funktionshinderpolitik.se,sjostadsbladet.se,fotbollsresultat.com,lansposten.se,dalabygden.se,sormlandsbygden.se,skaneplus.se###cookie-notice
aip.nu,lansposten.se,dalabygden.se,sormlandsbygden.se##body.cookies-not-set:style(overflow:unset!important)
akaviaaspekt.se##.article-list-item--native, a.article-topic__list-item[href^="/annons"]
aktieskolan.se##section.elementor-section:has-text(Huvudsponsorer & partners)
aktiespararna.se,alekuriren.se,tidningen.se,kurera.se,vinbanken.se##.native
aktuellhallbarhet.se,byggindustrin.se,dagensmedia.se,dagensmedicin.se,fastighetsnytt.se,resume.se,dagenssamhalle.se,market.se,dagligvarunytt.se,privataaffarer.se##article:matches-css(after, content:/Annonssamarbete/i)
aktuellhallbarhet.se,byggindustrin.se,dagensmedia.se,dagensmedicin.se,fastighetsnytt.se,resume.se,dagenssamhalle.se,market.se,dagligvarunytt.se,privataaffarer.se##a[href^="/annons/"], a[href^="/native/"], .slot-module, .slot-articlemodule
aktuellhallbarhet.se,byggindustrin.se,dagensmedia.se,dagensmedicin.se,fastighetsnytt.se,resume.se,dagenssamhalle.se,market.se,dagligvarunytt.se,privataaffarer.se##div[class^="css-"]:matches-css(content:/Annons/i):upward(article)
aktuellhallbarhet.se,byggindustrin.se,dagensmedia.se,dagensmedicin.se,fastighetsnytt.se,resume.se,dagenssamhalle.se,market.se,dagligvarunytt.se,privataaffarer.se##div[class^="css-"]:matches-css(min-height: /420px|400px|320px|312px/)
aktuellsakerhet.se##a[href*="reklamsamarbete"]:upward(.td_block_wrap)
aktuellsakerhet.se##.block-title:has-text(Reklamsamarbete):upward(.td_block_wrap)
aktuellsakerhet.se##.block-title:has-text(Reklamsamarbete):upward(.td_block_wrap) + rs-module-wrap:remove()
aktuellsakerhet.se##.front-slider-reklamsamarbete, .category-gastkronika-reklamsamarbete, .front-top-reklamsamarbete
aktuellsakerhet.se##.td-adspot-title-span:upward(1)
aktuellsakerhet.se,borattforum.se,sjostadsbladet.se##.td-a-rec
alandstidningen.ax##.revive-wrapper, div[id^="block-views-block-editorial-ads"], div[id^="block-blockbanner"]
alekuriren.se##div[id^="aleku-"], #carouselVideoAd, #carouselVideoAdMobile, .native-bg, .casino
aletorget.se,alingsastorget.se,almhulttorget.se,alvestatorget.se,amaltorget.se,angelholmtorget.se,arbogatorget.se,arvikatorget.se,askersundtorget.se,askersundtorget.se,avestatorget.se,bastadtorget.se,bengtsforstorget.se,bjuvtorget.se,bodentorget.se,bollebygdtorget.se,bollnastorget.se,borastorget.se,borlangetorget.se,botkyrkatorget.se,bromollatorget.se,eksjotorget.se,enkopingtorget.se,eskilstunatorget.se,eslovtorget.se,fagerstatorget.se,falkenbergtorget.se,falkopingtorget.se,faluntorget.se,filipstadtorget.se,flentorget.se,forshagatorget.se,gallivaretorget.se,gavletorget.se,gislavedstorget.se,goteborgtorget.se,gotenetorget.se,gotlandtorget.se,hagforstorget.se,hallsbergtorget.se,hallsbergtorget.se,hallstahammartorget.se,halmstadtorget.se,haningetorget.se,harnosandtorget.se,harrydatorget.se,hassleholmtorget.se,hebytorget.se,hedemoratorget.se,helsingborgtorget.se,herrljungatorget.se,hoforstorget.se,hoganastorget.se,hoortorget.se,horbytorget.se,huddingetorget.se,hudiksvalltorget.se,hultsfredtorget.se,hyltetorget.se,jonkopingtorget.se,kalixtorget.se,kalmartorget.se,karlshamntorget.se,karlskogatorget.se,karlskogatorget.se,karlskronatorget.se,karlstadtorget.se,katrineholmtorget.se,kavlingetorget.se,kiltorget.se,kirunatorget.se,klippantorget.se,kopingtorget.se,kramforstorget.se,kristianstadtorget.se,kristinehamntorget.se,krokomtorget.se,kumlatorget.se,kungalvtorget.se,kungsbackatorget.se,laholmtorget.se,landskronatorget.se,leksandtorget.se,lidkopingtorget.se,ljungbytorget.se,ljusdaltorget.se,ludvikatorget.se,luleatorget.se,lundtorget.se,lyckseletorget.se,lysekiltorget.se,malmotorget.se,mariestadstorget.se,markarydtorget.se,marktorget.se,moratorget.se,nackatorget.se,nassjotorget.se,norrtaljetorget.se,nybrotorget.se,nykopingtorget.se,nynashamntorget.se,olandtorget.se,olofstromtorget.se,orebrotorget.se,orebrotorget.se,ornskoldsvikstorget.se,orusttorget.se,osbytorget.se,oskarshamntorget.se,ostersundtorget.se,osthammartorget.se,partilletorget.se,piteatorget.se,ronnebytorget.se,saffletorget.se,salatorget.se,sandvikentorget.se,sigtunatorget.se,simrishamntorget.se,sjobotorget.se,skaratorget.se,skellefteatorget.se,skovdetorget.se,skuruptorget.se,soderhamntorget.se,sodertaljetorget.se,sollefteatorget.se,sollentunatorget.se,solnatorget.se,solvesborgtorget.se,staffanstorptorget.se,stenungsundtorget.se,stockholmtorget.se,strangnastorget.se,stromstadtorget.se,sundsvalltorget.se,sunnetorget.se,svenljungatorget.se,tabytorget.se,tanumtorget.se,tidaholmtorget.se,tierptorget.se,timratorget.se,tingsrydtorget.se,tjorntorget.se,tomelillatorget.se,torsbytorget.se,tranastorget.se,tranemotorget.se,trelleborgtorget.se,trollhattantorget.se,trosatorget.se,uddevallatorget.se,ulricehamntorget.se,umeatorget.se,uppsalatorget.se,vallentunatorget.se,vanersborgtorget.se,varatorget.se,varbergtorget.se,varnamotorget.se,vasterastorget.se,vasterviktorget.se,vaxjotorget.se,vellingetorget.se,vetlandatorget.se,vimmerbytorget.se,ystadtorget.se##.collapse.row.jobb.annonslista,#sponsored,#banners-right,.mittenbanner,#banners-top,#banners-bottom
alexandrabylund.se,helahisingen.se,sportsnews.se,xn--sporthnt-5za.se###af-preloader
alghundklubben.com#@#.category-annons:not(body):not(html)
alkompis.se##app-ads, .cdk-overlay-container
alkompis.se##.cdk-global-scrollblock:style(overflow-y: initial !important; position: unset !important;)
allaaktier.se##div[id^="ad-"]
allabolag.se##article:has(.advert__mark)
allabolag.se###company-card_top-banner, .lwad
allabolag.se##.strossle-widget:upward(div[style^="min-height"])
allas.se,elle.se,femina.se,hant.se,mabra.com,residencemagazine.se,svenskdam.se,motherhood.se##article.grid:has(a[href="/creative-studio"])
allas.se,elle.se,femina.se,hant.se,mabra.com,residencemagazine.se,svenskdam.se,motherhood.se##article.grid:has-text(/annonssamarbete/i)
allas.se,elle.se,femina.se,hant.se,mabra.com,residencemagazine.se,svenskdam.se,motherhood.se##article[data-type="native"], .ag-product-wrapper, .product-carousel__container, .shop_carousel, .editorsPick, div[class^="strossle-widget-"], .ad-min-height, a.cts-impression-item[data-cts-label*="banner"], section[data-cts-label="affiliate-carousel"]
allas.se,elle.se,femina.se,hant.se,mabra.com,residencemagazine.se,svenskdam.se,motherhood.se##a.js_commercial-text--link-text:upward(.jwplayer_video-videoArea):remove()
allas.se,elle.se,femina.se,hant.se,mabra.com,residencemagazine.se,svenskdam.se,motherhood.se##a:has([data-type="Sponsored"])
allas.se,elle.se,femina.se,hant.se,mabra.com,residencemagazine.se,svenskdam.se,motherhood.se##div.wings-gray-200:has-text(Annons)
allas.se,elle.se,femina.se,hant.se,mabra.com,residencemagazine.se,svenskdam.se,motherhood.se##p:has-text(ANNONS:)
allas.se,elle.se,femina.se,hant.se,mabra.com,residencemagazine.se,svenskdam.se,motherhood.se##+js(aeld, blur, i.focusPlayerElement)
allas.se,elle.se,femina.se,hant.se,mabra.com,residencemagazine.se,svenskdam.se,motherhood.se##+js(aeld, scroll, t.view.updateBounds)
allas.se,elle.se,femina.se,hant.se,mabra.com,residencemagazine.se,svenskdam.se,motherhood.se##+js(href-sanitizer, a[href*=".io/c/"], ?u)
allatvkanaler.se##.gda, .cookie-notification
allsvenskan.se##a[href*="track.adform"]
alltforforaldrar.se###partnerMenuContainer, #partnerMenuContainerFiller
alltforforaldrar.se##.spons-artc, a[href^="/native/"]
alltforforaldrar.se##.unslider-wrap.unslider-carousel>li:has(.preamble-category:has-text(/^annons/i))
alltforforaldrar.se,di.se,upphandling24.se,bytbil.com,sverigesnatur.org,tv24.se,nyan.ax##.panorama
alltomarbetsmiljo.se##main > div:not([id]):not([class]):has(a[href$="nyhetsbrevet"])
alltomarbetsmiljo.se##.bg-native
alltomburgare.se##.newscolumn:has(a[href$="/sponsrat/"])
alltomelbil.se###zox-lead-top-wrap
alltomelbil.se##:is(.p-list, div[class*="post-"]):has(a[href*="/annons"])
alltomhif.se##a:has-text(/betting|utan registrering|casino/i):upward(article, .slide-item):remove()
alltomhif.se##.sek-module-inner a[target="_blank"]
alltomkungligt.se###banner-holder
alltomnorrtalje.se##.allto-widget, .allto-before-content, .allto-after-content, article[class*="sponsrad"]
alltomsallskapsspel.se##.bannersRight
alpresor.se###toast-container
altinget.se##a[href^="/sponsrade"]
antagning.se,universityadmissions.se###cookiebanner
arbetaren.se##.text-sm:has-text(/annons/i):upward(.border-b, a[target])
arbetet.se,tidningenelektrikern.se,fastighetsfolket.se,handelsnytt.se,ka.se,sekotidningen.se##.Container:not(.ContentItem-content):has([data-controller="ad"])
arbetet.se,tidningenelektrikern.se,fastighetsfolket.se,handelsnytt.se,ka.se,sekotidningen.se##.Teaser--native, .o-native, [data-controller="ad"], div[id^="consent-"]
arjeplognytt.se##.metaslider
arjeplognytt.se##p:has-text(ANNONS):upward(.et_pb_text)
arkitekten.se##div[id^="consent-"]
arkitekten.se##html:style(--scrollbar-width:initial!important)
arkitekten.se##.MediaWrapper-content:style(opacity:unset!important)
arkitektur.se##article:has(.Entry-sponsored)
arkitektur.se##[class*="panorama"]
artbannersplus&task=show
assistanskoll.se###annons
atl.nu,landlantbruk.se,land.se##a[href*="/atl-tv-annons/"], [class^="Ad_"], div[class^="WidgetCTASticky"]
atl.nu,landlantbruk.se,land.se#@#.ad-unit:not(.text-ad):not(.textads)
atl.nu,landlantbruk.se,land.se,di.se,expressen.se,dn.se###didomi-host
aurumforum.se##span:has-text(Annons):upward(2)
autolife.se###Banners
automation.se,verkstadstidningen.se,transportnytt.se,datormagazin.se##.a-wrap
autonytt.se###main > .col-links
autonytt.se##.label:has-text(/sponsrad/i):upward(a)
autonytt.se##.sidebar_content:has(a[href*="casino"])
autonytt.se,sv.picmix.com,tekniknytt.se##.leaderboard
autopower.se##.card:has(.adsbygoogle)
avanza.se#@#a[title="LeoVegas"]
aventyrsresor.se,travelnews.se##.newsletter-popup
babyhjalp.se##.elementor-widget[data-settings*="sticky_"], div[id^="babyhjalp_panorama"], div[id^="babyhjalp_mobil"], div[id^="stagi"]
bakasockerfritt.se###cookiescript_injected_wrapper
bandyfeber.com##article:has(a[href*="/annons-"])
bandyfeber.com##.slide-entry-excerpt:has-text(/annons:/i):upward(.avia-content-slider)
bandyfeber.com##.widget_sp_image, a[title^="ANNONS"], .inner_sidebar .widget_text, .entry-content a[href*="utm_campaign"]
banners$image,domain=travsport.se|gavletravet.se
baraenkakatill.se##.post-item__tag:has-text(/spons/i):upward(li.post-item)
barnistan.se,welma.se##.newsletter, a[onclick*="adClick"]
barnistan.se,welma.se,ingenjorsjobb.se##.cookie-notice
barnsemester.se##.puffLine, .d-flex > div[style*="min-height"], div[style="overflow-x: hidden;background-color:rgb(250,250,250);width:320px;min-height:200px;"], div[style="overflow-x: hidden;background-color:rgb(250,250,250);width:320px;min-height:320px;"]
barometern.se,blt.se,bt.se,kristianstadsbladet.se,olandsbladet.se,smp.se,sydostran.se,trelleborgsallehanda.se,ut.se,ystadsallehanda.se,vxonews.se,vaxjobladet.se,nsk.se,klt.nu##div:has-text(/^Annons/):upward(a)
barometern.se,blt.se,bt.se,kristianstadsbladet.se,olandsbladet.se,smp.se,sydostran.se,trelleborgsallehanda.se,ut.se,ystadsallehanda.se,vxonews.se,vaxjobladet.se,nsk.se,klt.nu##div[class*="AdWrapper"]:upward(1)
barometern.se,blt.se,bt.se,kristianstadsbladet.se,olandsbladet.se,smp.se,sydostran.se,trelleborgsallehanda.se,ut.se,ystadsallehanda.se,vxonews.se,vaxjobladet.se,nsk.se,klt.nu##div[class*="fluffy-Overlay"]:has(img[src*="-ad/"], img[src*="Checkout"])
barometern.se,blt.se,bt.se,kristianstadsbladet.se,olandsbladet.se,smp.se,sydostran.se,trelleborgsallehanda.se,ut.se,ystadsallehanda.se,vxonews.se,vaxjobladet.se,nsk.se,klt.nu###root > div:first-child:matches-css(position: fixed)
barometern.se,blt.se,bt.se,kristianstadsbladet.se,olandsbladet.se,smp.se,sydostran.se,trelleborgsallehanda.se,ut.se,ystadsallehanda.se,vxonews.se,vaxjobladet.se,nsk.se,klt.nu##.component_guide-ads, #fullpage-ad-portal, div[style="min-height: 302px;"]
barometern.se,blt.se,bt.se,kristianstadsbladet.se,olandsbladet.se,smp.se,sydostran.se,trelleborgsallehanda.se,ut.se,ystadsallehanda.se,vxonews.se,vaxjobladet.se,nsk.se,klt.nu##:is([id*="_panorama"],[id*="_mobil"]):upward(div[display="block"])
barometern.se,blt.se,bt.se,kristianstadsbladet.se,olandsbladet.se,smp.se,sydostran.se,trelleborgsallehanda.se,ut.se,ystadsallehanda.se,vxonews.se,vaxjobladet.se,nsk.se,klt.nu##:is([id*="_panorama"],[id*="_outsider"],[id*="_insider"],[id*="_mobil"]):upward(1)
battregolf.se##article.elementor-post:has(a[href*="casino"], a[href*="bonus"], a[href*="betting"], a[href*="/noje/"])
battregolf.se##.elementor-element[data-widget_type="image.default"]
battrestadsdel.se###top-banner-mobile, .apd-text, .apds_main, .entry-priomaker, [class^="dls-"], .csmi
battrestadsdel.se,flashback.se,leta.se###top-banner
beernews.se##.cookie-consent-wrapper, #takeover-outer
bergsmannen.se,tidningenbyggmaterial.se##.ann-puff, .headerLinks
besoksliv.se##a[href*="sponsrat-innehall"], div[class$="-promotion"]
bestchampagne.se##aside.section-sm
bettips.se##.bettips-am
bettips.se,borskollen.se,se.azrhymes.com##.top-banner
biblioteksforeningen.se##body:style(opacity:1!important)
biblioteksforeningen.se,psykologiguiden.se,rabattsok.se###cookie-bar
bike.se##.post-block-style:has(a[href*="/annons"])
bildobubbla.se##.annonser
bilresaieuropa.se###header-image, #block-2
bilresaieuropa.se##.widget-title:has-text(/spons/i):upward(.widget_text)
bilsport.se##fl-gdpr, fl-panorama-top, fl-newsletter-popup
bilsport.se##.includingFeaturedSliderArticle:has(.native-mark)
bilwebben.ax##.front #secondary-content-wrapper, .banner-wrapper, .content-prefix-banner-wrapper
bioenergitidningen.se##article:remove-class(closed)
bioenergitidningen.se###cookieinfo
biostock.se,hejauppsala.com,svenskfilmdatabas.se,bredband.se##.wt-cli-cookie-bar-container
biostock.se,tobaksfakta.se##.pum-open:style(overflow:auto!important)
birthday.se##.datax
bjuvsweek.se##.carouselbanner-wrp
blocket.se##.placement_panorama, .blocket-placement, div[style="height: 240px;"], [class*="offering-info-box"], [data-id="placement_panorama"], div[class*="BannerLink"]
bohuslaningen.se,stromstadstidning.se,markposten.se,harrydaposten.se,partilletidning.se,sttidningen.se,molndalsposten.se,kungalvsposten.se,kungsbackaposten.se,alingsastidning.se,ttela.se,gp.se,hallandsposten.se,hn.se,mellerudsnyheter.se##.c-ad__panorama, .c-ad__insider, #outsiderTop, div[data-k5a-pos^="panorama"]
bokadirekt.se##a:not([href*="bokadirekt.se"]):not([href^="/"]) img
bokadirekt.se##.ReactModalPortal:has(a[href="/articles/cookies"])
bokmassan.se,svenskamassan.se##.cookie-law
boktugg.se##.elementor-section:has(.sponsor, .elementor-post.category-sponsrat)
boktugg.se##[id^="boktu-"]
boneo.se##.article-top-advt
boneo.se##.slick-slide:has-text(/sponsra/i)
booli.se###outer
borattforum.se##.meta-info-container:has(a[title*="Sponsrad artikel"])
borskollen.se##a:has(.sponsored)
borskollen.se##img[src*="/borskollen_newsletter"]:upward(1)
borskollen.se##.adlabel:upward(1)
borskollen.se##.colorized:has-text(/annons/i):upward(a)
borskollen.se##.elevated-button:has-text(/^Cookie/):upward(.container)
borskollen.se##.label:has-text(/annons/i):upward(1)
borskollen.se##.main > div[class^="jsx-"]:last-of-type:has(img[src*="borskollen_appen"])
borskollen.se##.outer:has(img[src$="ad_label.png"])
borskollen.se##.sponsored-chip:matches-css(display: block):upward(a)
borskollen.se##.wrapper > div[class^="jsx-"] > .outer:has(a[href*="casino"])
borskollen.se##[id^="borskollen_small"], [id^="borskollen_large"], .featured-link, .app-store-box, #borskollen_desktop-side, #borskollen_desktop-panorama, div[id^="borskollen_mobile-detaljsida"]
borssnack.di.se##.bn_advertisement__panorama, .bn_advertisement__container
borsvarlden.com##article:has(.border-sponsored)
borsvarlden.com##.label:has-text(/annons/i):upward(.highlighted-article-block)
borsvarlden.com##.sponsored-articles-container, .nav-sep-blink, .annons-label, .index-side-banner-wrapper, .index-top-banners-wrapper, .fullwidthbanner-container, .banner-wrapper
bovision.se##a:has(.ad-mark)
bovision.se##.banner-image
bovision.se##.blog-article-card:has(.sponsor-mark)
brafiler.se###header-banner, #cboxOverlay, #colorbox, .adv-inner, #sidebar-banner
brafiler.se##.rlt-top-pro:has(a[href*="casino"])
branschaktuellt.se##span:has-text(Sponsrad):upward(.article)
branschaktuellt.se##.popup-signup, .takeover
branschkoll.se##div[id^="brans-"], .widget-sponsored-post
branschstegen.se##.container:has(a[href*="casino"])
branschstegen.se##[class*="sponsored"], #watcherPop, .modal-backdrop
breakit.se##section[class*="Article_layout"]:has(section[class*="Sponsored"])
breakit.se##[class*="sponsored"], [class*="Sponsored"], [class*="LivepodPuff"], .videoAd, .js-video-ad, [class*="AdkContainer"], div[class^="LivewrappedContainer_root"]
brollopstorget.se##.bt-article:has(a[href*="/annons/"])
bukefalos.se,thaisnack.se,rollspel.nu,husbilsklubben.se,friaordet.org,xn--lnforum-exa.se,ihusbil.se##.u-bottomFixer
bulletin.nu##div[class*="section-preview"]:has-text(/betalt samarbete/i):upward(4)
bulletin.nu##[class^="newsletter-subscribe"], div[class^="cookie-message"], div[role="presentation"]
bulletin.nu,inredningsarkitektur.se,fof.se,allas.se,elle.se,femina.se,hant.se,mabra.com,residencemagazine.se,svenskdam.se,motherhood.se,aftonbladet.se,lchfarkivet.se,kollega.se,folkofolk.se,skyscanner.se,dagensarena.se,bokadirekt.se,barometern.se,blt.se,bt.se,kristianstadsbladet.se,olandsbladet.se,smp.se,sydostran.se,trelleborgsallehanda.se,ut.se,ystadsallehanda.se,vxonews.se,vaxjobladet.se,nsk.se,klt.nu,samnytt.se,sjofartstidningen.se##body:style(overflow:initial!important)
bussmagasinet.se###page > div:not(.left):not(.right)
bussmagasinet.se###titlebanner
bussmagasinet.se,byggteknikforlaget.se,dialasen.com,torbjornstips.se,backpacking.se,kanadaresa.se,usa.se,sporthalsa.se,ravarumarknaden.se,livetsgoda.se,opulens.se,radiotreby.se,nyadagbladet.se,fiskemagasinet.se,etunanytt.se##.textwidget a[target="_blank"]
butikstrender.se##a[target="_blank"] picture, div[data-settings*="sticky"], div[id^="butik-"]
butikstrender.se##body > .elementor > .elementor-section:first-child:has-text(Annons)
byggahus.se##a.click-track, img.click-track:remove-class(click-track)
byggahus.se##a.click-track-attachment-preview, img.click-track-attachment-preview:remove-class(click-track-attachment-preview)
byggahus.se##body.forum-logged-out .svartalistan-results-login-required:style(height: unset !important;)
byggahus.se##img[data-click-track]:remove-attr(data-click-track)
byggahus.se##+js(aeld, /adblockDetector|adsInserted|partnerExternalLinkClick/)
byggahus.se##.bbImageWrapper--preview.active img:style(-webkit-filter:none!important; filter:none!important; transform:none!important; -webkit-transform:none!important;)
byggahus.se##.block-ad, #cookie-consent-dialog, a[href^="/partner/"], .threadMatchedContent, #svartalistan-login-required-overlay
byggahus.se,expressen.se,filmtopp.se,destination.se,spokbloggen.nu,folkhalsasverige.se,foretagsverige.se,forskningsverige.se,motorbibeln.se,hallbarhetsverige.se,tillvaxtsverige.se,grillbibeln.se,kampenmotcancer.se,bolagsfakta.se,affarsvarlden.se,affarerinorr.se,viivilla.se##.ad-container
byggfaktadocu.se##.pop_box
byggfakta.today,citymark.today,hotellorestaurang.se##.cookie_popup_box
byggipedia.se##aside .textwidget:has-text(/sponsr|samarbetspartners/i)
byggipedia.se##*:style(user-select: auto !important;)
byggipedia.se##+js(acs, document.onkeydown, e)
byggipedia.se##+js(acs, document.onkeypress)
byggipedia.se##+js(acs, frames, oncontextmenu)
byggipedia.se##+js(acs, jQuery, contextmenu)
byggipedia.se##+js(set, ai_set_cookie, noopFunc)
byggipedia.se##.code-block:has(.adsbygoogle)
byggipedia.se##.protect_contents-overlay, .ai_widget
byggkontakt.nu##a:has-text(/poker|casino|kasino|betting/i):upward(li)
byggnadsarbetaren.se##[class^="siteAds"], .siteAlerts, #gan-popup
byggteknikforlaget.se###text-2.widget_text, .header-widget-area
byggvarlden.se,omtanke.today##a[href*="/annons/"], .newsletter-popup-content-overlay, .newsletter-popup, .ai-viewports
byggvarlden.se,omtanke.today##.post:has(a[href*="/annons/"])
bytbil.com##html,body:style(overflow: auto !important;)
bytbil.com###privacyModal
bytbil.com##.available-services
cafe.se,kingmagazine.se##.card-partner:upward(1)
cafe.se,kingmagazine.se,mestmotor.se##.card-partner, .partner
campingsverige.se##.banner_window, .banner_label, .card_veckans_pryl, .bg_camping_se
campingsverige.se##.post_sponsrad_label:upward(1)
camping.se##.ads-above-header, .ads-teaser, .paragraph--type--ad-script, div[about*="/annons/"], a[href*="/sv/annons"]
canariajournalen.se##.highlighted:has(.advertisement)
cannabisifokus.se##div[id^="canna-"]
cannabis.se##+js(aopw, Cookies)
cannabis.se##.header-ads-wrapper, .ai-adb-hide, .ai-sticky-widget, .hampaonline
cannabis.se,biostock.se,snowmobile.se,tobaksfakta.se,dagenslogistik.se,magasinetkonkret.se,skaneplus.se,battrestadsdel.se##.pum-overlay
carup.se##div[id^="carup-"]
casinoguiden$image,domain=samnytt.se|samnytt.nu
casino$domain=pirkt.se
casino-utan-$image
cfosvepet.se##.recent-post-item:has(a[href="#"]:not(.w-condition-invisible))
chefstidningen.se##[id^="block-views-ad"], .modal-container
chef.se##.Cookie-notice, .Product-modal, .Offer-popup, .Toaster
chef.se,fokus.se##.Blurb--native
cineasten.se###text-6, .theiaStickySidebar .category-uncategorized
cineasten.se##.ajax_loader
computersweden.se##.nativo
computersweden.se##.latest-content__card-secondary:has(.nativo)
com.se,~www.com.se##html::before:style(content: "OBS! VARNING! Om denna sida är en butik så är det förmodligen en bluffbutik. Detta är ett meddelande från det svenska filtret i din annonsblockerare." !important; font-size: 18px !important; font-family: sans !important; background-color: red !important; color: white !important; padding: 6px !important; width: 100% !important; display: block !important; text-align: center !important;)
conpot.se##div:has-text(ANNONS):upward(article:not([id]))
conpot.se##+js(set, square_array1, null)
conpot.se##+js(set, square_arraytop, null)
cookaholic.se###loftloader-wrapper
cookie-consent$domain=upphandling24.se
cornucopia.se###sponsrade-lankar:upward(aside) + aside.widget_block
corren.se,folkbladet.se,mvt.se,nt.se,vt.se,vimmerbytidning.se,kuriren.nu,nsd.se,norran.se,pt.se,ekuriren.se,strengnastidning.se,kkuriren.se,sn.se,eposten.se,unt.se,helagotland.se,kindaposten.se,gotlandjustnu.se##ad-iris-sunt-ad-wrapper, ad-block, .native, ad-full-page-block, a[href^="/native"], widget-family, widget-memorial, widget-marknadsguiden, widget-jobb-plus, a.puff-primary-link[href*="/erbjudande/"], .ad-hidden, iris-puff-native
corren.se,folkbladet.se,mvt.se,nt.se,vt.se,vimmerbytidning.se,kuriren.nu,nsd.se,norran.se,pt.se,ekuriren.se,strengnastidning.se,kkuriren.se,sn.se,eposten.se,unt.se,helagotland.se,kindaposten.se,gotlandjustnu.se##iris-subscribe-footer
corren.se,folkbladet.se,mvt.se,nt.se,vt.se,vimmerbytidning.se,kuriren.nu,nsd.se,norran.se,pt.se,ekuriren.se,strengnastidning.se,kkuriren.se,sn.se,eposten.se,unt.se,helagotland.se,kindaposten.se,gotlandjustnu.se,tv.nu,klart.se##.sp-message-open body:style(overflow:unset!important;position:unset!important;)
curateContext=affiliate$domain=aftonbladet.se
cykelframjandet.se##:is(article.tg-item, .lcp_catlist li):has(a[href*="/annons"])
cykla.se##.featured-post--sponsored, .grid-item--sponsored, #advert-once-banner-fullskarm
cykla.se#@#.advertisment
dagensarena.se##.popup
dagensinfrastruktur.se,nyaprojekt.se,nordiskaprojekt.se,svenskbyggtidning.se,grontsamhallsbyggande.se##.g-single, a[onclick*="banner"], a[onclick*="advert"], .adrotate
dagensjuridik.se##strong:has-text(/^senaste nytt från våra partners/i):upward(.card--muted)
dagensjuridik.se##.outher-sidebar, a[href*="/annons/"], .dj-inline-ad
dagenslogistik.se##div.g, .top-banner
dagenslogistik.se##small:has-text(/annons/i):upward(.elementor-column)
dagensps.se##a[href*="/ps-partner"]:upward(section.cat-post-widget)
dagensps.se##a[href*="/ps-partner/"], .ad-links-module, .dagensps_ad, a[href*="ut.dagensps.se"][target], .bottom_banner, .leftsidebanner, .c-external-notice
dagensps.se##div[class^="bg-"]:has(a[href="/ps-partner"])
dagensps.se##.container:has(.dagensps_ad)
dagensps.se##.postbox:has(.sponsored_post)
dagensps.se##:is(.text-text-secondary, span.font-bold):has-text(ANNONS):upward(2)
dagenstech.se##a[href^="https://dagenstech.se/articles/"]:upward(1):has-text(SPONSRAT)
dagenstech.se##.banner-desk, .banner-mob
dagenstech.se##.text-right:has-text(ANNONS)
dagenstv.com##.slick-slide:has-text(/casino/i)
dagenstv.com,kolla.tv##.grid-add-container
dagensvimmerby.se,dagensvastervik.se,dagenskalmar.nu,dagenshultsfred.se##body:style(margin-top: 0 !important;)
dagensvimmerby.se,dagensvastervik.se,dagenskalmar.nu,dagenshultsfred.se##.panoramaAnnons, .JobAdDiv, .annonsKolumn, .insideAd, .ingressAd, .familyAds, .annonsWrapper
dagens.se##.item:has(.prebid, div[data-ad-unit-id], a[href*="casino"])
dagen.se##.video-annons, .native-box, .arcad-block-container
danskaspraket.se##.rightcol
darkside.se##a[href*="?aktion=bannerclick"]
datormagazin.se##a:has-text(/^annons/i)
datormagazin.se##div[id^="dator-"]
datormagazin.se##.heading:has-text(/samarbete/i):upward(.elementor-widget-smartmag-featgrid)
datormagazin.se##.td-big-grid-post:has(a[href*="/samarbete/"])
datormagazin.se##.td_module_wrap:has(a[href*="/annons/"])
dayviews.com##.frontPageBox--links
da.se##.Advert
deliquate.se##[id^="ads300"], [id^="linkcat-"]
densistavilan.se##div[data-advadstrackid]:upward(.x-bar-footer)
densistavilan.se##h3:has-text(Advertorial):upward(1)
densistavilan.se###fancybox-wrap, div[id^="densi-"]
dental24.se##.fp_banners, .cypress-popup_newsletter
dental24.se##.post-box:has(.sponsored)
designbase.se##html,body:style(overflow:unset!important;)
designbase.se##.banner-hidden, .z-newsletter-modal, .z-newsletter-popup
desktop-banner$image,domain=bokadirekt.se
destination.se,sistaminuten.se##+js(set-cookie, CM_cookieConsent, 0)
devote.se##article.tile:has-text(/annons|spel|casino|kasino/i)
devote.se##div[data-losjs^="borka"]:upward(1)
devote.se##+js(aeld, click)
devote.se##.slick-slider
devote.se,familjeliv.se##div[style*="height: 244px;"]
digitalavykort.se##.rightdiv p:has-text(/casino|kasino|lån|betting|odds|lotto/i)
digitalfotoforalla.se,iform.se,pctidningen.se,varldenshistoria.se##li:has(.content-label:has-text(/annons/i)):remove()
digitalfotoforalla.se,iform.se,pctidningen.se,varldenshistoria.se##.scroll-message, .gallery-banner, .horseshoe, [data-ad-type], .bcm-banner
digitalfotoforalla.se,iform.se,pctidningen.se,varldenshistoria.se##.teaser:has(.teaser__cat--sponsorlabel)
digitalfotoforalla.se,pctidningen.se##.opacity-fade:style(opacity:1!important; transition:none!important; animation:unset!important;)
dinamediciner.se##.top-header:has(.adsbygoogle)
dinbyggare.se##article.category-leverantorer, div[style^="\[banner-style\]"]
dinbyggare.se##p[style="text-align: center;"]:has(a[target] > img)
dinbyggare.se##*:style(-webkit-touch-callout: default !important; -webkit-user-select: text !important; -moz-user-select: text !important; -ms-user-select: text !important; user-select: text !important;)
dinbyggare.se##+js(rmnt, noscript)
dinbyggare.se##+js(rmnt, script, /wccp_pro/)
dinbyggare.se##::selection:style(background-color:#007aff!important;color:#fff!important;)
dinvinguide.se##.contain:has(a[target="_blank"])
discoveringtheplanet.com##body:remove-class(unselectable)
discoveringtheplanet.com##html:style(user-select:unset!important; -moz-user-select:unset!important; -webkit-user-select:unset!important;)
discoveringtheplanet.com##+js(acs, disableEnterKey)
discoveringtheplanet.com##+js(acs, document.ondragstart)
discoveringtheplanet.com##.widget-title:has-text(/annons/i) + .textwidget
di.se##+js(set, getAdblockerStatus, noopFunc)
di.se##.di_panorama-wrapper, .site-header__panorama, .di_panorama__isAdLabel, .discount-box, .campaign-ad-box, .di_start__teaser-placeholder, .di_teaser-flak-planbokskoll, .di_teaser-flak-container--native, .native-box, .bandit-box__teaser--native, a[href*="/brandstudio"], .service-box, .brand-studio-box, .native-article, .listing-box-native
di.se##.market-start-top + div:not(.market-container__wrapper)
djungeltrumman.se##strong:has-text(/samarbete|sponsrat/i):upward(li):remove()
djungeltrumman.se###sponsored-posts, #right-banners, .banner-wrapper, .top-banner-label, .banner-label
djungeltrumman.se##.label-sponsored:upward(#latest-slider a):remove()
djungeltrumman.se##.post:has(.label-sponsored)
dn.se##body:style(position:unset!important;overflow-y:scroll!important;)
dn.se##.article--native, .teaser-card--native, .ds-teaser--native, #dnse-popup
dn.se##.campaign-holder
dn.se,di.se##video:remove-attr(data-auto-play)
dn.se,di.se##.teaser-native
dn.se,di.se,expressen.se,atl.nu,landlantbruk.se,land.se,hd.se,sydsvenskan.se,allehanda.se,tidningenangermanland.se,arbetarbladet.se,avestatidning.com,bblat.se,dalademokraten.se,fagersta-posten.se,gd.se,lt.se,ltz.se,na.se,norrteljetidning.se,nynashamnsposten.se,op.se,salaallehanda.com,st.nu,tidningenharjedalen.se,vlt.se,falkopingstidning.se,jp.se,skaraborgslanstidning.se,skovdenyheter.se,smalandsdagblad.se,smalanningen.se,smt.se,tranastidning.se,vastgotabladet.se,vetlandaposten.se,vn.se,bandypuls.se,ljusdalsposten.se,ljusnan.se,soderhamnskuriren.se,ht.se,moratidning.se,borlangetidning.se,falukuriren.se,sodran.se,nyaludvikatidning.se,skd.se,nvp.se,nuiosteraker.se,netdoktorpro.se,popularhistoria.se,aktuellhallbarhet.se,byggindustrin.se,dagensmedia.se,dagensmedicin.se,fastighetsnytt.se,resume.se,dagenssamhalle.se,market.se,dagligvarunytt.se,privataaffarer.se,barometern.se,blt.se,bt.se,kristianstadsbladet.se,olandsbladet.se,smp.se,sydostran.se,trelleborgsallehanda.se,ut.se,ystadsallehanda.se,vxonews.se,vaxjobladet.se,nsk.se,klt.nu,illvet.se,pctidningen.se,digitalfotoforalla.se,iform.se,varldenshistoria.se,slakthistoria.se##body.didomi-popup-open:style(overflow:unset!important)
doktorn.com##.js-banner-wrapper
doktorn.com##.js-cookie-disclaimer
doon.se##.doon-promotion, a.link[target="_blank"]
driva-eget.se##.sponsored_content
dust2.se##html[data-impression-tracking-endpoint]:remove-attr(data-impression-tracking-endpoint)
dust2.se##.main-page-content:style(background-image:none!important;)
dust2.se##.target-banner, div[data-type="BANNER"]
dykarna.nu###rightbanners
edgeflyfishing.com###g-header, #g-aside, #g-sidebar, div[data-role="sidebarAd"]
ehandelstips.se##:is(li, article):has([href*="/sponsradeartiklar/"])
ehandel.se##.aside-list--heading:has-text(/^sponsra/i):upward(.aside-list)
ehandel.se##.code-block:has-text(/annons/i)
ehandel.se##.commercial-row, .aside-image-with-link, .post-container-sponsored, aside a[href*="/branschnyheter/"]
ekonominyheter.se###lblock-ads
ekonominyheter.se##.td-fix-index:has(a[href*="casino"])
ekonominyheter.se,autonytt.se,undervarttak.se,aftonbladet.se,lesscarbs.se,hockeybladet.nu,matinspo.se##a[href*="/track.adtraction."]
electronic.se##.content aside.column-narrow:last-of-type
elektronikforumet.com##td > a[target="_blank"] img
elevspel.se##div#cookie_wrapper
elevspel.se##div[class*="-unit"]:has(a[href="/medlem/plusmedlem.html"])
elevspel.se##+js(rmnt, script, cloned.removeAttr)
elle.se##section.c-native_banner:upward(2)
emocore.se###main > #home_start_div ~ .m_t.box:nth-last-child(-n+2)
emocore.se###sticky-panorama-container, #mob-wrap
energi.se##.advertisement--item
eniro.se##article:has(#marketing)
eniro.se##div.rounded-4xl:has(a[href$="/firma#marketing"])
epochtimes.se##.fixed.bottom-0
esportare.se##a[href*="utm_campaign"]
esportare.se##em:has-text(Annonser):upward(2)
esportsacademy.se###preloader
espressomedia.se##div[id^="espre-"], .category-native
espressomedia.se##.penci-block-vc:has([href*="casino"])
etc.se##.adaptive:upward(1)
etc.se##.paywalled.hidden:style(display:unset!important)
etc.se##[data-controller="ad-container"], .bg-gradient-white
etn.se,uppsalanyheter.se,rotter.se##.banneritem
etunanytt.se##.textwidget:has-text(ANNONS)
etunawebben.se##+js(nostif, ad)
europaportalen.se##.view-multiply-top
eu-cookie$domain=skidspar.se
eventeffect.se###secondary > .widget:nth-child(2)
eventeffect.se,executiveeffect.se,saleseffect.se##.partnerartikel, #sidebar-ads-right, #nyhetsbrev-pp-wrapper__container
eventeffect.se,executiveeffect.se,saleseffect.se##.post-teaser:has(a[href$="/annons/"])
evergreengarden.se##article.elementor-grid-item:has-text(reklamsamarbete)
evertiq.se##+js(acs, $, banner_loader)
evertiq.se##.cc-container, [data-gabnr], #carpet
evertiq.se,fz.se##.bnr
everysport.com##div[id^="everysport_sky"], img[alt="X3000"], img[alt="Casinofeber"]
everysport.com##:is(div[id^="everysport_pano"], div[id^="everysport_rektangel"]):upward(1)
exakt24.se##section[data-ha-element-link*="kampanj"], .elementor-element-686a3aa6, .elementor-popup-modal
existenz.se##.link:has(a[href*="bannerid="])
existenz.se##.wm-nopop, #main > p[style^="color"], #slidebox
existenz.se,funfunfun.se,elektronikforumet.com##a[href*="bannerid"]
expo.se##div.flowy-wp-protected-content:remove-class(flowy-wp-protected-content)
expo.se##p.has-text-align-center:has-text(Annons:)
expo.se##.ad-image, .bottom-popup
expressen.se##.campaign
expressen.se##a:remove-attr(data-t-label)
expressen.se##a:remove-attr(data-t-type)
expressen.se##a[href*="/spel.exp"], a[href*="/lanapengar.exp"], a[href*="/rabattkoder.exp"], a[href*="/annons"], .match-betting, .discount-ad, .b-ad__caption, .pressrelease-teaser, .widget-ad-marker, .widget-ad-marker + a, .promotion-banner, .widget--collaboration, .rotator--external, a[data-click-track*="prisjakt"], .linked-image-widget a[href*="/kampanj/"], .linked-image-widget a[href*="lifestyle.expressen.se"], #premiumAdWrapper, .tapet-popup-overlay, .outsider-ads, .teaser > a[href*="/kampanj."], .teaser > a[href*="/brandstudio"], .teaser > a[href*="/brand-studio"], figure[data-article-data*="/sponsrat"], figure[data-article-data*="/annons"], figure[data-article-data*="/brand-studio"], .teaser--native, .native-article
expressen.se##strong:has-text(/^annons:/i):upward(p)
expressen.se##.html-widget > div[style^="text-align: center; font-size: 10px;"]
expressen.se##.tapet-popup-js-no-scroll, .tapet-no-scroll:style(overflow-y:initial!important; position:unset!important;)
expressen.se##.teaser:has(a[href*="/annons"], a[href*="/brandstudio"], a[href*="/brand-studio"], a[href*="/kampanj."], a[href*="/lanapengar."], a[href*="/rabattkoder."], a[href*="/spel.expressen.se"], .vignette--svg + a[href*="teknikensvarld."], .teaser__bottom--ad-marker)
expressen.se,di.se,nsk.se,skd.se,nvp.se,nuiosteraker.se,barometern.se,blt.se,bt.se,kristianstadsbladet.se,olandsbladet.se,smp.se,sydostran.se,trelleborgsallehanda.se,ut.se,ystadsallehanda.se,corren.se,folkbladet.se,mvt.se,nt.se,vt.se,klt.nu,vimmerbytidning.se,kuriren.nu,nsd.se,norran.se,pt.se,ekuriren.se,strengnastidning.se,kkuriren.se,sn.se,eposten.se,unt.se,helagotland.se,kindaposten.se,folkbladet.nu,vk.se,vasterbottningen.se,mellanbygden.nu,nordsverige.se,lokaltidningen.nu,vasterastidning.se,mitti.se,thelocal.se,byrum.se,sverigespringer.se,recept.se,viivilla.se,mestmotor.se,babyhjalp.se,fragbite.se,ibnytt.se,realtid.se,cafe.se,kingmagazine.se,vxonews.se,vaxjobladet.se,alekuriren.se,nyheter24.se,svenskgolf.se,golfing.se,gotlandjustnu.se,familjeliv.se,praktisktbatagande.se,norrahalland.se,lokalti.se,lchfarkivet.se,alltforforaldrar.se,idrottensaffarer.se,vf.se,hjotidning.se,kt.se,kt-kuriren.se,sla.se,mariestadstidningen.se,filipstadstidning.se,fryksdalsbygden.se,nwt.se,arvikanyheter.se,nkp.se,saffletidningen.se,provinstidningen.se,dalslanningen.se,nlt.se,skaraborgsbygden.se##+js(json-prune, autoplay)
extraextra.se##.sm-text:has(.adsbygoogle)
extrakt.se,macken.xyz,dialasen.com,lakartidningen.se,ordmedzcxy.se###cmplz-cookiebanner-container
familjehemsbanken.se,familjehemmet.se###cookieNotice
familjeliv.se##article:has-text(/annons:/i)
familjeliv.se##a[href*="/kampanj/"], .flm-kampanj
familjesidan.se##.cookies-wrapper
fastighetssverige.se##a[href*="/banner/out/"], .bnr_box, div[class^="panel"][style*="lightgoldenrodyellow"]
fastighetssverige.se##.featured-article:has(.badge-partner-text)
fastighetstidningen.se##.adspace, a[class*="annons"]
fasting.nu##body:style(display:unset!important)
feber.se,tjock.se##f-internallinks-new:has-text(Annons)
feber.se,tjock.se##+js(nosiif, checkGDPRInt)
feber.se,tjock.se##+js(set, dovideostuffAD, noopFunc)
feber.se,tjock.se##.burt-unit, .art_ad, adline, f-panorama, f-deals, #rpPopular, #maxetiseFull, #outsider, [data-ad="true"]
festivalinfo.se##a[title*="Casino"], #top-content
festivalinfo.se##.node-news:has(a[href*="casino"])
fightermag.se##article:has(a[href*="betting"], a[href*="casino"], a[href*="kasino"], a[href*="/gastskribent/"])
fightermag.se##a[href*="/sponsra"], #partners
filatelisten.se##:is(a[target="_blank"]:not([href^="/"], [href*="filatelisten.se"])):upward(section)
filmparadiset.se##.jnews-cookie-law-policy, a[href*="casino"], .custom-html-widget a[target="_blank"]
filmtipset.se##em:has-text(/sponsrad/i):upward(.row.news)
filmtipset.se###topslider-wrapper + .container > .sidebar, .sidebar a[target="_blank"], .sidebar a[href*="casino"], .sidebar a[href*="betting"], .sidebar a[href*="automater"]
filmtipset.se##.news:has-text(casino)
filmtipset.se##.row.news > div[style^="border"]:last-of-type
filmtopp.se##body:style(overflow:initial!important)
filmtopp.se##.cooperation-banner__container, .takeover-desktop, .takeover-mobile, #discover-banner
finanstid.se##.tdm-descr:has-text(/casino/i)
findit.se##+js(set, testPrebid, noopFunc)
findit.se##.banner-wrapper, .col-banner
firstclassmagazine.se###leader-wrap, #rpwe_widget-2
firstclassmagazine.se##.feat-cat:has-text(/annons/i):upward(a)
firstfoto.se##article.status-publish:has-text(/annonssamarbete/i)
firstfoto.se###cookie-consent-banner
fisheco.se###page-section-2, #page-section-24, .add-special-banner, .g-single
flamman.se##.Banner, .TakeOverBanner, .CookieNotice, div#popup
flashback.org###top-banner-container, #top-banner-wrapper
flashback.org##+js(nostif, #top-banner-container)
flashscore.se##.boxOverContent--a, .otPlaceholder, .seoAdWrapper, .adsbackground-wrapper, .prematchOddsBonus__bonus, .prematchLink[target], .detailLeaderboardSkeleton
flm.nu##.spons
flygtorget.se###PreHeader
fl-net.se##a:has-text(/lån|casino|kasino/i):upward(p)
fl-net.se###spopup
fl-net.se##.thumbnail:has([data-revive-zoneid])
fn.se###cookie
fodertipset.se##.fodertipset-org-banner
fof.se###CybotCookiebotDialog, #CybotCookiebotDialogBodyUnderlay
fof.se##.mediaconnect-protected-content .Carousel:style(opacity:unset!important;)
fof.se,elinstallatoren.se,spraktidningen.se,modernpsykologi.se,vvsforum.se##.mediaconnect-protected-content, .mediaconnect-protected-content--show:style(max-height: unset !important; overflow: unset !important;)
fof.se,elinstallatoren.se,spraktidningen.se,modernpsykologi.se,vvsforum.se##.mediaconnect-protected-content::after:style(background: unset !important;)
fokus.se##.sesamy-protected-content.active::after:style(background:unset!important;)
fokus.se##.sesamy-protected-content:style(max-height:unset!important;overflow:unset!important;)
folkofolk.se##div[class^="MuiDialog-root"]
foodfolder.se###myModal, .adImage
foretagande.se##article:has(.sponsored-text)
foretagande.se##div.article:has(a[href$="artiklar-i-samarbete"])
foretagande.se##div[id*="panorama"], .panorama-pos
foretagsverige.se,forskningsverige.se,motorbibeln.se,hallbarhetsverige.se,tillvaxtsverige.se,grillbibeln.se,kampenmotcancer.se,folkhalsasverige.se##:is(div[class*="vicky-whitebox"], .vicky-category-label, .vicky-video-infobox-label, .vicky-post-headline-container__category__inner):has-text(/spons/i):upward(a, .carousel-caption, .featurette, article)
forexgruppen.se##div[data-widget_type="image.default"] a:not([href*="forexgruppen.se"], [href^="/"]), .widget_media_image a:not([href*="forexgruppen.se"], [href^="/"])
forexgruppen.se##+js(noeval-if, adbEnableForPage)
forexgruppen.se,datormagazin.se,skogen.se##.cky-consent-container
forni.se##.recent-articles:has(.collaboration-brand)
forskning.se##.cli-modal
forstasidorna.se##body.tingle-enabled:remove-class(tingle-enabled)
forstasidorna.se##.tingle-modal--visible
forum.mustangclubsweden.org##a[href*="&do=advertisement&ad=1"]
forum.robsoft.nu##td[valign="middle"] > a[target="_blank"]
forum.robsoft.nu##.cookie-box
forvaltarforum.se##.ff_sponsored_articles, .widget_sow-image a[target="_blank"], .ff_banners_widget_widget
forvaltarforum.se##.ticker-title:has-text(/partner/i)
forvaltarforum.se##.ticker-title:has-text(/partner/i) + .mh-section
fotbolldirekt.se,hockeysverige.se,innebandymagazinet.se##.c-announcement:has(.c-label--sponsored)
fotbolldirekt.se,hockeysverige.se,innebandymagazinet.se##.c-announcement:has-text(/annons/i)
fotbolldirekt.se,hockeysverige.se,innebandymagazinet.se##.pdcw-item--code:has(img[src*="bet365"])
fotbolldirekt.se,hockeysverige.se,innebandymagazinet.se,motivation.se,fiskejournalen.se,alba.nu,padeldirekt.se,dagensopinion.se##.annons
fotbolldirekt.se,hockeysverige.se,innebandymagazinet.se,padeldirekt.se##.site-partnevisment, .h-background--sponsored-light, .row .text-center img, a[href^="https://hubs.la"], .c-partners, iframe[srcdoc*="_ad_div"], .annons-text
fotbollskanalen.se##a:has(.brand-info__ad-text)
fotbollskanalen.se##.brand, .desktop-ad-web, a[href*="telia.se/privat/tv/sport"] img, .mobile-ad-web, .ad-banner
fotbollskanalen.se##:is(.notice__tag_sponsored, .notice__tag):has-text(/sponsrat/i):upward(1)
fotbollsresultat.com##h2:has-text(Spel och dobbel) ~ p
fotbollsthlm.se##.fotbollsthlm-image-container:has(.fotbollsthlm-ad-link)
fotbolltransfers.com##div[class^="ad"], a[href^="https://ads."], .header_sponsored, .fresnel-greaterThanOrEqual-panorama, .fresnel-lessThan-panorama, a[rel*="sponsored"]
fotbolltransfers.com##div[style^="min-height"]:has(div[id^="fotbolltransfers_mpu"], div[id^="fotbolltransfers_mobil"])
fotbolltransfers.com##img[src*="/images/annonser/"]:upward(1)
fotbolltransfers.com##.smallNewsCategory:has-text(/sponsr/i):upward(.smallNewsLink)
fotboll-tv.se##.SMBoxContentBanner, a[data-gaevent*="action=bookmaker_odds"], #ouibounce-modal, .SMGameAtomSingleGameOddsComponent
fotboll.com##.header-static-lg, .fp-partner, .xs-ad, .bo-wrapper, #betsid, .news-banner-mini, .xs-cblock, .cookie_consent_bar, #odds, a.bellows-target[href*="/svenskaspel"], a.bellows-target[href*="/betting"]
fotboll.com,allsvenskan.se,superettan.se,swebbtv.se,hastnet.se##.smartbanner
fotosidan.se##+js(aeld, contextmenu, , showCopyrightBox)
fotosidan.se##.subArticlesponsored, div[style="width:300px;float:right;"], div[style="float:right;width:300px;"], #partner-box, .adbox-label
fotosidan.se,merinfo.se,allsvenskan.se,tasteline.com,jaktojagare.se,chefstidningen.se,realtid.se,norpan.se,moviezine.se,jaktjournalen.se,byggvarlden.se,omtanke.today,akademikern.se,socionomen.se##.ads
fragbite.se##.category:has-text(/spons/i):upward(article)
fragbite.se##.tn, .zooKeeper, #scraper, .subHeadSponsors
framtid.se###siteflash, #customer-link-container
fraser.nu##div[aria-label="Annonser"]
freeride.se##img[src*="/sponsor/"] + br + .boxlogo, .sidebar-front .boxen
freeride.se##.mark:has-text(/spons/i):upward(.post)
freeride.se##.sidebar-front .widget_text.dark ~ p
freeride.se##.visible-xs:has(a[href*="casino"])
freeride.se,gamereactor.se,happyride.se##.sponsor
fria.nu,stockholmsfria.se##[class*="annonser"], #cboxOverlay, #cboxWrapper
frihet.se##.CookieBar
frilagt.se##.elementor-location-header section.elementor-element:first-child
friluftsframjandet.se##[id^="ad-"]
funktionshinderpolitik.se##.topp-banner, .annons-mark
funnygames.se,nyckelspel.se##.slot-container
fuska.nu##span:has-text(/casino/i):upward(li)
fuska.nu##.list:has(a[href*="casino"])
fuska.se##.alert-success
futsalmagasinet.se##div.modal-cacsp-backdrop, div.modal-cacsp-position
futsalmagasinet.se##html.modal-cacsp-open:style(position:unset!important)
futsalmagasinet.se##span:has-text(/annonserat innehåll/i):upward(.td_block_wrap)
futsalmagasinet.se##.wp-block-column > h2:has-text(/annonser/i) ~ p
futsalmagasinet.se,newsvoice.se,obsid.se##aside.widget:has(a[href*="casino"])
fz.se##.article-facebook
fz.se##.card:has(.article-sponsored, a[href*="/sponsrat"])
fz.se##.fp-carousel .fpci-kicker:has-text(/^sponsr/i):upward(.fpc-item)
fz.se,fssweden.se##+js(set, adblock, false)
gaffa.se##a[href*="/annonser/"], a[href*="/sponsrat-"], div[id^="cncpt-"]
gaffa.se##h4:has-text(/sponsrade länkar/i):upward(.link-list)
gaffa.se##.article-overview__col:has(.gpt--loaded)
gamereactor.se##video:remove-attr(data-autoplay)
gamereactor.se###cookielawwarning, #eventad, [id^="sky"], [id^="ad_lead"], a[rel="sponsored"], .external_div_bigVideoAd, #mpu, #leftToLogo, .itsanad, div[class^="ad_Bumper"], div[style="min-height: 600px; margin-bottom: 20px;"], div[id^="ad_"], div[class^="preAd_"], div[class^="ad_smartphbig"], .adMobileBig, div[class^="preMobileBig"], .external_div_videoAd, .ad_mobilebigwrap
gamereactor.se###grtvbelt_Sponsored:upward(1)
gamereactor.se##+js(set, adblockEnabled, falseFunc)
gamereactor.se##.ad_interscroller:upward(.wrapper)
gamereactor.se##.colHomePlayer:has([data-slotads="videoad"]):remove()
garaget.org##+js(rmnt, #text, casino)
garaget.org##.gorgad, .gorg-side-content > div.small:nth-last-child(2), .gorg-side-content .bottom-buffer ~ *
gasetten.se##.footer-widgets .widget_block li
gasetten.se,fotbollsthlm.se##article:has-text(/är en annons/i)
gasetten.se,fotbollsthlm.se##.footer-links, .fotbo-target
gentlemannaguiden.com##.advertising, .sidebar .widget_text, .sidebar .widget_media_image, .has-post-thumbnail.category-okategoriserade
glassakademin.se##[class^="adverts-"]
gmfk.nu###site-preloader
godare.se##a p[class^="hyperion-css"]:has-text(INNEHÅLLER ANNONSLÄNKAR):upward(li, a.internal-link)
godare.se##h3:has-text(Annons):upward(1)
godare.se##.godare-ad-element, a[href*="/brand-studio"], a[href*="/brandstudio"], .recipe-ad, a[href*="utm_campaign"][data-test-tag="external-link"]
golfguidenonline.se###citadela-infobar
golflivet.se##a[href*="/annonssamarbete/"], .deals_block_wrapper, .ai-close-fit
golf.se##.partner-area
google.se##div.g:has(a[href*=".com.se/"]):has-text(/återförsäljare|rea|garanti|lågt pris|nöjd|priser|shop|bra pris|kläder|skor|outlet|frakt|butik|betala/i)
google.se##h2:has-text(Annons):upward(#topstuff)
google.se##mobile-promo
goteborgsgolfaren.se##.sgpb-popup-overlay, #sgpb-popup-dialog-main-div-wrapper, .et_pb_gallery
goteborg.com##body:style(overflow-y:initial!important)
goteborg.com##.cookie-popup, .overlay
grandtech.se##aside#secondary:has(.adsbygoogle)
grillbaronen.se##a[href*="/click."], #block-2, #block-4
grillbaronen.se##.post:has(a[href*="casino"], a[href*="kasino"], a[href*="betting"])
grillbloggen.nu##.rstbox
guideAds$xmlhttprequest,domain=barometern.se|blt.se|bt.se|kristianstadsbladet.se|olandsbladet.se|smp.se|sydostran.se|trelleborgsallehanda.se|ut.se|ystadsallehanda.se|vxonews.se|vaxjobladet.se|nsk.se|klt.nu
guldkanalen.se##div.grid_container[style*="height:240px;"]
gynning.net##.sponsored-notification:upward([id^="post-"])
hallakonsument.se##section[aria-label="Kakinformation"]
hallbartbyggande.com##div[id^="hallb-"]
hallbyhandboll.se,skiljebosk.nu##.cookiePush, .stickyFollow, .sponsorGroup__item
halsafitness.se,yogaworld.se,cyclingplus.se##h3:has-text(/samarbete/i):upward(.post-wrap)
halsafitness.se,yogaworld.se,cyclingplus.se##.sticky-sidebar, #gdpr-container, .slick-carousel
hammarbyfotboll.se##body[data-modal-open]:style(overflow-y:unset!important;)
hammarbyfotboll.se###seasonalTakeover, div[class*="sponsorBarContainer"], div[class*="footerSponsors"], .slick-slide a[target="_blank"]
handbollskanalen.se##.hb-adlabel, [id^="hb-"], .ad-placement-side, p > a[target="_blank"]
handelsnytt.com##.headerannons, .sidebarannonsseg, .footerannons
handel.ax###topadmob
hant.se,svenskdam.se##div.text-center:has(div[ad-placement])
happypancake.se##a[href*="casino"]:upward(1)
happypancake.se###__next > div > div.bar:first-child
happypancake.se##+js(aopr, Object.prototype.adUnits)
happyride.se##li:has(a[href*="/category/sponsrat/"])
happyride.se##.col-sm-4 > div[class]:has(a[href*="casino"], a[target="_blank"])
happyride.se,freeride.se##.anm1-container, [class^="anp"], [class^="ans"], .box.evergreen
hastnet.se##div[style*="--mobile-height"]:has(div[id^="div-gpt"])
hastnet.se##.add-wrap, .listings-search-ads, .right_panel, #pmg-widget-root
hbwebben.se##.elementor-widget-container > a > img
hd.se,sydsvenskan.se,allehanda.se,tidningenangermanland.se,arbetarbladet.se,avestatidning.com,bblat.se,dalademokraten.se,fagersta-posten.se,gd.se,lt.se,ltz.se,na.se,norrteljetidning.se,nynashamnsposten.se,op.se,salaallehanda.com,st.nu,tidningenharjedalen.se,vlt.se,falkopingstidning.se,jp.se,skaraborgslanstidning.se,skovdenyheter.se,smalandsdagblad.se,smalanningen.se,smt.se,tranastidning.se,vastgotabladet.se,vetlandaposten.se,vn.se,bandypuls.se,ljusdalsposten.se,ljusnan.se,soderhamnskuriren.se,ht.se,moratidning.se,borlangetidning.se,falukuriren.se,sodran.se,nyaludvikatidning.se,skd.se,nvp.se,nuiosteraker.se,hbl.fi,vastranyland.fi,bbl.fi##[class*="teaser-native"], lcl-ad, .ad-welcome, .affiliate-links__container, .x-bonnier-news-links__container
hejaolika.se##p[style^="text-transform"]:has-text(/annons/i)
hejaolika.se##p[style^="text-transform"]:has-text(/annons/i) + .wp-block-kadence-posts
hejaolika.se##+js(acs, advads_passive_placements)
hejaolika.se##[class*="partnerinfostyle"], div[id^="hejao-"], .kb-advanced-image-link[target], .category-partnerinformation, .kt-modal-linkalign-center, .hejao-target
hejauppsala.com##:is(div[class^="u-text"], h2):has-text(/^Reklam$/):upward(section)
hejauppsala.com,bredband.se##.cli-barmodal-open:style(overflow:auto!important)
helahisingen.se###custom_html-15, .code-block img, .banner-promotions-wrapper
helgon.se##[id*="banner"], a[href^="https://ad."], a[href^="https://ad2."]
hellofresh.se##a[data-test-id^="top-banner-ad"], div[data-test-id="exit-intent-banner"], div[data-test-id="urgency-banner-modal"]
hemhyra.se##.pageCookies, #ad-insider1, #ad-insider2, #ad-mobil-1, #ad-mobil-2, #ad-mobil-3, #ad, #ad1, #ad2, #adform-outstream, .ad__text, .entry__ad, .entry__related__sponsored, .module__sponsored
hemmafixbloggen.se##.post-item:has(.sponsor-summary)
hemmanytt.se###sa_slider_shortcode
hemmanytt.se##.annonsnotis + span + span + div.td-pb-row:has(a[href*="adtr.co"])
hemnet.se##body:style(overflow:unset!important)
hemnet.se##div[data-testid="living-cost-logos-section"]:has(span[aria-label="annons"])
hemnet.se##span:has-text(/annons från/i):upward(div[class^="ArticleContent_articlePage"])
hemnet.se###ad_unit_placeholder, div[class^="Panorama_panoramaAd"], .listing__panorama-banner, .broker-banner, div[class^="BrokerBanner"]
hemnet.se##:is(article, li):has([class*="SponsoredLabel"], .article-card__sponsored-text)
hemnet.se##:is(div[class^="Carousel"], #top_listing):has(div[class^="PaidPlacementLabel"])
hemnet.se##:is(small, span):has-text(/sponsrad/i):upward(article, li, a)
hemtrevligt.se##div[id^="hj-"], div[id^="ik-"]
hemtrevligt.se##.article:has(.annons)
hifitorget.se##.billboard-style, .between-posts
hifitorget.se##.row[style*="height"]:has(.adsbygoogle)
hippson.se##.main-article-container:has-text(/Sponsrad Artikel/i)
hitta.se##a[data-trackimp][target], .hitta-map .integration-txt, .section-details--alb, [class*="dummyAd"], [class*="StyledAdSlot"], [data-bind*="Ad"], div[class^="GraphicAd_"], [class*="adContainer"], [id*="_panorama"], [id*="_skyscraper"], div[style="min-height: 250px;"], div[data-track="displayplacering-customer"], a[data-test="boostAdLink"], div[class^="style_bannerContainer"], [data-track="click-promotion-banner"], div[class*="adWrapper"]
hitta.se##div[id^="hitta_mobile_"].placeholder:upward(div[class^="height"], div[class^="style_breakout"])
hitta.se##[class^="styleManual_mainContentBox"] > div[style^="min-height"]:first-of-type
hockeybladet.nu##.td_mod_wrap a img[data-permalink], a[data-wpel-link="external"][onclick], a.td-lazy-img[target], a[href*="casino"]
hockeybladet.nu##.vc_row_inner:has-text(casino)
hockeyettan.se##.club-ad-item, .banner-row
hockeyguiden.com##.main-loader.loader-bg
hockeymagasinet.com##body:remove-class(modal-open)
hockeymagasinet.com##gdpr-alert
hockeynews.se##.items-center:has(a[target="_blank"])
horisontmagasin.se##small:has-text(/annons/i)
hotellorestaurang.se,citymark.today,byggfakta.today###bannnerContainer, #pop_overlay, .banner-s, div.featured
hrnytt.se##article:has(.sponsored-article)
hrnytt.se##.banner-box
hrsvepet.se##.mini-title-link:not(.w-condition-invisible):has-text(/sponsra/i):upward(1)
hrsvepet.se,cfosvepet.se##.cookie-banner, .desktopbanner
humorbibeln.se,newsner.com,sportbibeln.se,ettgottskratt.se,djurbibeln.se##.inline-share-buttons
hungrig.nu##.ui-widget-overlay, .ui-dialog
husbilsplats.se##div[id^="husbi-"]
husvagnochcamping.se##div[id^="husvagnochcamping-"], .ast-below-header-bar
husvagn.se,husbil.se##strong:has-text(/samarbete/i):upward(li.item)
husvagn.se,husbil.se##.ui-top-adversite, #optin-cover, #optin
ibnytt.se##h3:has-text(Speltips):upward(.widget)
ibnytt.se##:is(a[href*="casino"], a[href*="speltips"]):upward(.widget)
icagruppen.se##div[ng-controller="CookieConsentCtrl"]
icagruppen.se##div[ng-show*="isUiDisabled"]
ica.se,naringslivetvgl.se,dalarnasaffarer.se,stockholmsaffarer.se,jamtlandsaffarer.se,hallandsnaringsliv.se,sjuharadsnaringsliv.se##.banner-area
idrottensaffarer.se###header:style(height:unset!important;)
improveme.se##.banner-center, .banner-center ~ br, div[class^="ad-container"]
improveme.se##.flow_teaser:has(a[href*="casino"], a[href*="poker"], a[href*="cbd-olja"])
improveme.se##.wp-pagenavi:style(position:unset!important;z-index:unset!important)
inblick.se##div[class^="ads"]
indien.nu##.nyhetsochreseartiklar .views-row:has-text(/casino/i)
industrinyheter.se,dagensnaringsliv.se,infrastrukturnyheter.se,sportochfritidsnyheter.se,inredningsnyheter.se,byggnyheter.se,dagensfastigheter.se,stockholmsbyggnyheter.se,energinyheter.se,vindkraftsnyheter.se,solenerginyheter.se,jarnvagsnyheter.se,transportochlogistik.se,metallerochgruvor.se,papperochmassa.se,miningmetalnews.com##.insider-ads, [id^="mainadvertorial"], [id^="dfptag"], .block-advertorial, .block-views-blockconventus-info-articles-info-article-block, #dfp-tag-before_artikel, #dfp-tag-mobile_before_artikel, #block-views-block-leader-article
industritorget.se###pnlCookie, .campaign-top, .campaigns-right
inet.se##+js(set-cookie, allow-marketing-cookies, 0)
influens.se##strong:has-text(Annons:):upward(.code-block)
influens.se##.code-block-label:has-text(Annons:)
influens.se##[class*="ai-viewport"], .ai_widget, #cb-sidebar-h, .livewrapped, .livewrapped_mobil
ingenjorsjobb.se##body:remove-class(advert-take-over-active)
ingenjorsjobb.se##.advert-take-over
inkopsradet.se##div[id^="inkop-"]
innebandy.se##[class*="banner-container"], .sponsorsswipeblock
inredningsarkitektur.se##.article:has-text(/sponsrad artikel/i)
internetmedicin.se##[itemtype="https://schema.org/WPAdBlock"]
internetodontologi.se##.overlay
internetodontologi.se##+js(aeld, /contextmenu|keydown/, e.preventDefault)
ipo.se##.tag-sponsrad
itseniorerna.se###astroid-preloader
itseniorerna.se###redim-cookiehint-modal
it-finans.se,it-halsa.se,it-kanalen.se,it-pedagogen.se,it-retail.se,it-hallbarhet.se##a[onclick^="gtag"], .header-banner, .penci-featured-cat-custom-ads
it-finans.se,it-halsa.se,it-kanalen.se,it-pedagogen.se,it-retail.se,it-hallbarhet.se##.widget-title:has-text(/annons/i):upward(aside)
it-finans.se,it-halsa.se,it-kanalen.se,it-pedagogen.se,it-retail.se,it-hallbarhet.se,espressomedia.se##.penci-wrap-gprd-law
jaktjournalen.se##.activate-notifications-container.shown, .newsletter-popup-content-overlay, .newsletter-popup, [class*="ai-viewport"]
jaktjournalen.se##.post:has(.post__category--sponsored)
jaktojagare.se##div.cookie-warning-container, .mb-adarea
jaktplay.se##.jaktplay-ad
jaktsidan.se,edgeflyfishing.com###ipsLayout_mainArea > iframe
jarnvagar.nu##.et_pb_module:matches-css(before, content: "Annons:")
javligtgott.se##div[id^="ad-panorama"]:upward(.elementor-section)
javligtgott.se##.jet-popup
jobsinsweden.se##+js(set, eazy_ad_unblocker, null)
journalisten.se##.o-blockCarousel--placementAd, .o-blockArea__item--block-ad, .m-blockAd
kalender.se##.day-nav ~ a:not([href*="kalender.se"]), a:not([href*="kalender.se"]) img, div[style^="height:340px"], div[style^="height:110px"]
kalmar.nu###rb-cookie
kamrat.com###kadDiv, div[style="margin:25px 0;max-width:255px!important;"], #scrollAdj ~ *
kamrat.com##+js(set, showAds, false)
kamrat.com##+js(set, trap, noopFunc)
kardemummagumman.se###custom_html-2
karinrahm.se##.thb-page-transition-on:style(opacity:1!important)
karlskogavaxer.se##.elementor-heading-title:has-text(/annons/i):upward(.elementor-column)
karriarlakare.se##a:has(.annons-label)
karriarlakare.se##a[target][onclick], #cliSettingsPopup
karriarlakare.se,livinguppsala.se,battrestadsdel.se,butikstrender.se,forskning.se,vardfokus.se,varvat.se,smaspararguiden.se,aktuellsakerhet.se,maklarvarlden.se,kvartal.se,sjostadsbladet.se,tidningenridsport.se,cookaholic.se,vinliv.se,raa.se,svenskfilmdatabas.se,hejaolika.se,arbetsvarlden.se,hockeybladet.nu###cookie-law-info-bar
kartor.eniro.se##.e-banner
kb.se,dansportalen.se,hh.se##body:style(overflow:unset!important; position:unset!important;)
kb.se,dansportalen.se,hh.se##.sv-marketplace-sitevision-cookie-consent, .sv-cookie-consent-modal, .env-modal-dialog__backdrop, .env-modal-dialog__backdrop--in
kiacarclub.se##.forumlist-main-inner > div[style]
kiacarclub.se##.sidebar-block:has-text(/annons|sponsor/i)
kimura.se##a[href*="unibet.com"], a[href*="/kampanjer."], a[href*="utm_campaign"], div[class^="yw-"], a[data-wpel-link="external"][target="_blank"]
kingsizemag.se##a:has(.disclaimer-tag-img)
kingsizemag.se##div#video-overlay, div.sidebar_frame, #affiliates, #affiliates + .text, #popup-interstitial-overlay, .cu_banner, #interstitial-overlay, .kingsize-native
kittad.se##li:has(.kittad-label-sponsored)
kittad.se###header-top, div[data-hook="consent-banner-root"]
klart.se##body:remove-class(mega-loading)
klart.se##div[id^="sp_message_container"]
klart.se###overlay, a[rel*="sponsored"], .-panorama-ad-wrapper
klimatnytt.se##.tm-cookie-banner
knulla.se###cookie-popup
kobe.se##p:has-text(/annonser:/i):upward(.widget_block)
kobe.se##.post:has(a[href*="casino"])
kokaihop.se##body:style(overflow-y: auto !important;)
kokaihop.se##.ads-wrapper-main, .InterstitialModal
kokaihop.se##.cookieBarWrapper:remove()
koket.se##[class*="carousel_sponsored"]:upward([class*="carousel_item"])
koket.se##[class*="list_item_sponsored"], [class*="promotion_bottom_holder_wrapper"], [class*="beverage-recommendation_wrapper"], [class*="list_item_wide_sponsored"], [class^="ad_position"]
koket.se##[class*="sponsorLabel"]:upward([class*="mosaic_item_wrapper"])
kolla.tv##div[style^="position: fixed; left: 0px; top: 0px; width: 100%; height: 100%; z-index: 999;"]
kollega.se##.block--gamw
kolozzeum.com##td[width="305"], br + a[href*="/casino"]
kompanjoner.se##.site-loader
komponentkoll.se##.gdpr-wide
konsumentmagasinet.se##.pricerunner
kristendate.se##div[id^="adv"]
kristendate.se##.cc-banner.cc-bottom
kritiker.se##div.recad, div.adhor, div.stickyad
kritiker.se##iframe[allow]:remove-attr(allow)
kritiker.se##+js(set, checkAdblocker, noopFunc)
kritiker.se##+js(set, checkAdsBlocked, noopFunc)
kritiker.se##+js(set, premium, trueFunc)
kritiker.se##+js(set, p, true)
kulturama.se##.CookiePopup
kulturbloggen.com,schack.se##.sidebar .widget_custom_html
kultwatch.se##.js-preloader > .document, .js-preloader > .hero-section:style(opacity: 1 !important; visibility: visible !important;)
kurera.se##.pc-das, .newsletter-popup
kvalitetsmagasinet.se,miljo-utveckling.se,telekomidag.se,vdtidningen.se##article:remove-class(closed)
kvalitetsmagasinet.se,miljo-utveckling.se,telekomidag.se,vdtidningen.se###subscribe_splash, [class*="nativeadwidget"], .partnermedia, .annonswidget
kvartal.se##.email-popup-wrapper
kvartal.se##.square-format:has(.kv-ad-label)
kwiss.me##.square-item:has(.qz-quiz-sponsored)
lajvo.se###panoramaTop
lajvo.se##.postCard:has-text(/bonusar|casino|betting|spelbranschen/i)
lakartidningen.se##.screen-sm, .screen-md
lakartidningen.se,hockeynews.se,canariajournalen.se##.advertisement
landleyskok.se##.inpostbanner, .banner-leaderboard
langd.se##.single-entry__ads
lantbruksnytt.se###startpage-top-right, .ads_text + a, div[class*="square_rotate"], a[target="_blank"][rel="nofollow"], #ouibounce-modal
laromedia.se##img[alt="Annons"] + .img-flipper
lawline.se##[class^="CookiesModal"]
lchfarkivet.se##.lchf-modal--wrapper, div#beskrivning[style="font-size: 10px; text-align: center; color: #8E8C8C; max-width: 700px;"]
lektionsbanken.se,runnersworld.se##.footer-newsletter
lesscarbs.se##article:has(a[href*="/annonssamarbete/"])
lesscarbs.se##.elementor-image > a:not([href*="https://lesscarbs.se"]), a[href*="/affiliates/"], div[id^="1"][style*="250px"]
lesscarbs.se##.e-loop-item:has(div[data-eael-wrapper-link*="annonssamarbete"])
lesscarbs.se#@#.category-annonssamarbete:not(body):not(html)
leta.se###bookingcom-resor-wrapper, #aktuellaerbjudanden, #sky-left-wide, .topNavItem[href*="casino"], .topNavItem[href*="betting"], #bottom-splinks
levandehistoria.se##div[class^="CookieBar"]
lexbase.se##+js(cookie-remover, lmt)
lidingonyheter.se##.moban
lifeofsvea.se,quizza.nu,trendenser.se##.cookie-info
lindasbakskola.se,jennysmatblogg.nu,zeinaskitchen.se,filippoon.se##.panorama-sticky, .sticky-area, #ad-outofpage_dynamic
lindasbakskola.se,skk.se,realtid.se,viivilla.se,ungdomsfotboll.se##a[href*="/bit.ly/"]
linguee.se##div[class*="ad_container"], div[class*="_ads_"]
lira.se###cookies-accept
lira.se,danstidningen.se,slangopedia.se,tidningen.se###ads
listor.se##article.feed-item:has-text(/låna pengar|casino|betting/i)
listor.se##article:has(a[href*="/annons/"])
listor.se###ss-floating-bar, .top-ads-widget, .header-inner center, #sidebar-right .widget_custom_html
listor.se##:is(a[href*="casino"], a[href*="betting"], a[href*="poker"]):upward(.elementor-widget)
litteraturmagazinet.se###pageContainer > div:first-child:not([id]), #topContainer a:not([href="/"], a[href="/sitesearch"])
livesport.expressen.se##[class^="BauProvider"]
livetochdiabetes.se###text-3
livetsgoda.se##body:style(opacity:unset!important)
livetsgoda.se##.penci-rlt-popup
livetsgoda.se,betongforeningen.se,espressomedia.se,realtid.se,ordfrontmagasin.se,europaportalen.se,motorsportbladet.se,battregolf.se,nitroz.se,magasinethockey.se##a[target$="blank"] img:not([class^="tweet"])
livinguppsala.se##.fusion-post-content-container:has-text(/^annons/i):upward(article)
livsmedelsverket.se###CookieConsent
livsmedelsverket.se##.lock-scroll:style(overflow:unset!important)
livsstil.se##article:has(.ad)
livsstil.se##a[href*="campaign"][data-test-tag="external-link"], div[data-ad-subtype], [data-test-tag="prisjakt-carousel"]
livsstil.se##div[data-variants*="article-panorama"]:upward(1)
livsstil.se##h3:has-text(/^Annons$/):upward(1)
livsstil.se##p:has-text(/^kommersiellt innehåll/i):upward(article)
livsstil.se##p:has-text(/^kommersiellt innehåll|^annons$/i):upward(a)
livsstil.se,godare.se##[id^="adPlacement"]:upward(1)
ljudochbild.se##div[class^="col-md"][style*="border-radius"]:has(a[href*="/advertorial"])
ljudochbild.se###MoreLink_content-container:style(height:unset!important;)
ljudochbild.se###MoreLink_fade-out-div
ljudochbild.se##.adremark, .coofad, .popup-overlay, .hidead, .phoneads, .pricecomp, .offerz, .type-articleadvertorial, .adblock, .lbplussinfo, .popup-overlayx, a[href*="/advertorial"], a[href*="/advertorial"] + .textbox, .prisjakt, #stickleft, #stickright
ljudochbild.se##.thecontent, .entry-content:style(max-height: unset !important; overflow: initial !important; height: unset !important;)
ljudochbild.se##.wp-caption:style(display:initial!important)
ljungbysporten.se##section.widget_media_image, a[target="_blank"]:not([href*="ljungbysporten.se"])
ljuskultur.se##body.private:remove-class(private)
ljuskultur.se,bettips.se,spelo.se,skogsaktuellt.se,maskinbladet.se,entreprenadaktuellt.se,ja.se,husbilhusvagn.se,klassiker.nu,mopedgaraget.se,vibilagare.se,caroftheyear.se,automobil.se,endurobloggen.se,riksettan.net,fightermag.se,frillesasbandy.se,dh.se,djungeltrumman.se,skik.se,omni.se,campingsverige.se,eniro.se,svenskjakt.se,realtid.se,restaurangvarlden.se,naringslivetvgl.se,dalarnasaffarer.se,stockholmsaffarer.se,jamtlandsaffarer.se,hallandsnaringsliv.se,sjuharadsnaringsliv.se,nyheteridag.se,epochtimes.se,alekuriren.se,omniekonomi.se,sverigesindustri.se,onkologiisverige.se##.banner
ljuskultur.se,hrnytt.se,aapl.se,inredningsarkitektur.se,inblick.se,matklubben.se##.cookies
lokalguiden.se##.applicant-match-container, .banner-item
lokalnytt.se##.panoramaImageBox
lokalti.se##:is(img[src$="a_top.png.webp"], a[href*="casino"]):upward(section.elementor-section)
loppi.se##a[href="https://loppi.se/promotion"]:upward(.page__section)
loppi.se##.entry__teaser--promotion, .wpcnt, .sunt-widget, .lifeofsvea-widget
lovelylife.se##.elementor-image a[href]:not([href*="lovelylife.se"]) img
luleahockeyforum.com##main > div:first-child:has(.banniere)
lundagard.se###bdCheckAlso.bdCheckAlsoShow, .topBanner, #sidebar .widget_media_image
lundextra.se,huddingeextra.se,sundsvallextra.se,goteborgextra.se,sollentunaextra.se##.category-partners
lundgiants.se##.cookieAlert
lundgiants.se##strong:has-text(Detta är en annons):upward(.inner)
lundgiants.se###LoggaDiv:style(position:unset!important;)
lwcdn.com##+js(aeld, /^(?:adBlocker|contextmenu)$/)
lwcdn.com,alingsastidning.se,bohuslaningen.se,gp.se,hallandsposten.se,hn.se,stromstadstidning.se,ttela.se,kungsbackaposten.se,kungalvsposten.se,molndalsposten.se,partilletidning.se,sttidningen.se,markposten.se,harrydaposten.se,mellerudsnyheter.se##+js(json-prune, autoplay players.*.ga acl.ads players.*.autoplay)
lysekilsposten.se###archiveAdContainer, .casino-wrapper
m3.se,pcforalla.se,macworld.se##span:has-text(/sponsr/i):upward(article)
m3.se,pcforalla.se,macworld.se##+js(href-sanitizer, a[href*="/idg.digidip.net/"], ?url)
m3.se,pcforalla.se,macworld.se##.amazon_lightning_deals_wrapper
mabra.com,motherhood.se##article.grid:has-text(/annonssamarbete/i)
macken.xyz##a[target="_blank"]:not([href^="/"]):not([href*="/macken.xyz"])
macken.xyz##.et_pb_section:style(opacity:1!important; animation-duration:unset!important; animation-fill-mode:unset!important;)
magasinetparagraf.se###large_banner
magasink.se##[data-magasintrackbid]
maipenrai.se##.cWidgetContainer > ul > li:first-child, div[style*="border: 1px solid"] a[target="_blank"], div[data-role="sidebarAd"], a[href*="&ad="]
maklarvarlden.se##article:has(.sponsored-inlist)
maklarvarlden.se##.hustle-popup
maklarvarlden.se##.td-post-category:has-text(/spons/i):upward(2)
maklarvarlden.se##.td-pulldown-size:has-text(/spons/i):upward(3)
maltermagasin.se##.mh-sidebar, .mh-header-columns
maltermagasin.se##.widget_media_image:has-text(/annons/i)
maringuiden.se##.banner_hoger, .google_ads_mg_frontpage, .footerComercialDiv
marknadschefer.se##section.elementor-inner-section:has(.adsbygoogle)
marknadschefer.se##.elementor-column:has(.ekit-sticky)
marknadschefer.se##.elementor-widget-heading:has-text(/Sponsra|annons/i)
marknadschefer.se##.elementor-widget-heading:has-text(/Sponsra|annons/i) + .elementor-widget-post-block
marsta.nu##.outsider, .panel--naringsliv
matinspo.se##div:remove-class(with-ads)
matinspo.se##[id^="matin-"]
matkanalen.se###sidebar .widget_text
matmalin.se##div[id^="matma-"]
matochpyssel.nu##.loading:style(opacity:1!important)
matpriskollen.se###kd-preloader
matspar.se##div[style="z-index: 2000;"],div[style="z-index: 2000;"] + div
matspar.se###ad-panorama-category:upward(1)
matspar.se##+js(json-prune, payload.ads campaigns.*)
matspar.se##.overflow-hidden:style(overflow-y: initial !important;)
medibok.se##noscript:has-text(mdp-deblocker-js-disabled):remove()
medibok.se##style:has-text(body * :not):remove()
medibok.se##+js(acs, show_msg)
medibok.se##.annonsmellandiv, .annonssidadiv
megafonen.se##[data-article-sponsored="true"], .content-main-adwrapper, .campaign-sidebar
meningokockfonden.se###page_preloader
merinfo.se##article[data-customer]
mestmotor.se##.advInsideSticky
mestmotor.se##ul.wp-block-post-template:has(a[href*="/kategori/partner/"])
metalcentral.net##.bannergroupno-padding
metalcentral.net,egoinas.se###tm-top-a
metalcentral.net,rotter.se##.bannergroup
metromode.se##+js(href-sanitizer, a[href*="metromode.se/bouncer"], ?url)
metromode.se##.advert:upward(.slick-item):remove()
metromode.se##.b-topshop
metromode.se##:is(.b-card, .b-related__item):has(.advert)
mhis.se##.bg-grey-light:has(a[target="_new"])
milansverige.se##.elementor-image a[target="_blank"], .oc_cb_wrapper, .elementor-widget-image a[target="_blank"]
miljomat.se##[id^="Annons"]
minhembio.com##div[style="height: 120px;"]:not([id]):not([class])
minimalisterna.se##p:has-text(/i samarbete med/i):upward(.post)
missatsamtal.se##.nosnaj
missatsamtal.se##.comment:has(.nosnaj)
mitti.se##h3:has-text(/annons/i):upward(.image-component-unprocessed)
mitti.se###cruncho_now_iframe:remove()
mitti.se##+js(set, NWS.config.enableAdblockerDetection, false)
mitti.se##.profile-native
mitti.se,cafe.se,praktisktbatagande.se##+js(aeld, scroll, helpers.scroll(id))
mmabetz.se##.desktop-homepage-ad, .desktop-main-ad, .latest-betting-campaigns, .best-casino-section, .top-casino
mmanytt.se##.front-banner, .front-banner-cover, #text-2, [class*="sponsrat-inlagg"], a[href*="://kampanjer."], .ohmbet_link, a[href*="adsrv.eacdn.com"], .jeg_postblock + .wpb_content_element, .spelbolag-text, .adbox, .fight-odds-aggressive
mmanytt.se##.img-featured-posts-image:has(a[href$="/annons/"])
mmanytt.se##.tablepress:has(a[href*="expekt"])
mobilanyheter.net##a[href*="rocketpot.io"], a[href*="casino"], a[href*="betting"], .a-wrap
mobilanyheter.net##+js(set, ai_run_scripts, noopFunc)
mobil.se,kamerabild.se##a[href^="/partner"]
mobil.se,kamerabild.se##.markupbox:has(a[href*="casino"])
modernalivet.se##body.modal-active:style(overflow:unset!important)
modernalivet.se##h3:has-text(/annons/i):upward(.sidebar-widget)
modernalivet.se##.excerpt:has-text(/annons/i):upward(article)
modernalivet.se##.modal-wrap, .slide-in-box
modette.se##.true_native_block
morotsliv.com##.et_bloom .et_bloom_flyin_center, a[href*="/?utm_medium=affiliate"], a.bigblue[target]
motivation.se##.card:has(.sponsored)
motivation.se##.sponsored-item, [class*="banner"], .outsider
motormagasinet.se,dagenshandel.se,food-supply.se,plastnet.se,habit.se,woodnet.se,foodnet.se,transportnet.se,processnet.se,packnet.se,verkstaderna.se,medtechmagazine.se,recyclingnet.se,rt-forum.se,uochd.se,lifesciencesweden.se,fri-kopenskap.se,cleannet.se,framtidensbygg.se,entreprenad.com,metal-supply.se##.box-of-announcement, a[href*="campaign"][target="_blank"], div[class*="rotating-"], #bottombanner, #promoPopup, .modal-backdrop, .newsletterPopUp
motorsportbladet.se##:is(article, li):has(a[href*="casino"], a[href*="kasino"])
moviezine.se##strong:has-text(ANNONS:)
moviezine.se###home_ans, [name="article-advertisment"]
moviezine.se##.inner_article:has-text(/sponsrat|annons/i)
mygatemagazine.se##.textwidget:has-text(Annons)
mytaste.se##body.modal-active.modal-open::before, body.modal-active::before:style(opacity: unset !important; content: unset !important;)
mytaste.se##div[id*="panorama_"], [class^="affiliate-container"], .site-header__panorama, .alert-cookiedisclaimer
mytaste.se##.recipe-modal[data-state=default] .modal-container.open, .recipe-modal[data-state=panorama] .modal-container.open:style(padding-top: 0 !important;)
mytaste.se##.site-wrapper[data-state=panorama], .site-wrapper[data-state=default]:style(padding-top: 40px !important;)
mytaste.se##[id^="Modal_plugin"]
m.yelp.se##div[class^="overlay-color-cohort"]:has(a[aria-label="Download the Yelp app"])
m.yelp.se##html:style(overflow:unset!important; position:unset!important;)
naringslivetvgl.se,dalarnasaffarer.se,stockholmsaffarer.se,jamtlandsaffarer.se,hallandsnaringsliv.se,sjuharadsnaringsliv.se###dr-preloader
naringslivetvgl.se,dalarnasaffarer.se,stockholmsaffarer.se,jamtlandsaffarer.se,hallandsnaringsliv.se,sjuharadsnaringsliv.se##.header-menu__wrapp:style(position:unset!important)
naringslivetvgl.se,dalarnasaffarer.se,stockholmsaffarer.se,jamtlandsaffarer.se,hallandsnaringsliv.se,sjuharadsnaringsliv.se##.header-top__wrapp, .article-item__banner
naringslivetvgl.se,dalarnasaffarer.se,stockholmsaffarer.se,jamtlandsaffarer.se,hallandsnaringsliv.se,sjuharadsnaringsliv.se##.list-article__item-inscription:has-text(/sponsrat innehåll/i):upward(.list-article__item)
naringslivetvgl.se,dalarnasaffarer.se,stockholmsaffarer.se,jamtlandsaffarer.se,hallandsnaringsliv.se,sjuharadsnaringsliv.se##:is(.slick-slide, .article-item__line-bottom):has(.sponsored-badge)
naringslivetvgl.se,dalarnasaffarer.se,stockholmsaffarer.se,jamtlandsaffarer.se,sverigesindustri.se,hallandsnaringsliv.se,sjuharadsnaringsliv.se,onkologiisverige.se##.cookies-popup
narkive.se##div[onimpression]
nasdaqomxnordic.com##+js(acs, $, shuffle)
naturvetarna.se##.Advertisement
netdoktor.se,netdoktorpro.se##.article-list__item__link--sponsored, .ispanorama, #Popup, .ElementAdvertisement
netflixguiden.se##div.lboard, div.instream-dynamic, #top-area-promo, div.sidebar div.sticky, .promo, .lboard-desktop, .lboard-mobile, #bottom-sticky-promo
news55.se##div.container:has(a[href="/author/news55-partner/"])
news55.se##div.justify-center:has(div[id^="news55_pano"], div[id^="news55_tws"], div[id^="news55_mobil"])
newsner.com,humorbibeln.se,sportbibeln.se,ettgottskratt.se,djurbibeln.se###wsfb-container, .share-buttons, .ad-space
newsner.com,humorbibeln.se,sportbibeln.se,ettgottskratt.se,djurbibeln.se##.ssp_divider:has(.sponsored-bar)
newsvoice.se##h3:has-text(/annons/i) + .textwidget
newsvoice.se##.sponsrad, .sponsradcol1
ng.se###nativendo-mainfeed:upward(1):remove()
ng.se##.secondary-sidebar > .panel-pane:last-child
ng.se##.view-partner-articles, [class*="sponsored-article"], .tertiary-bottom, div[class*="nojesguidenads"]
nogg.se##:is(td[rowspan="2"][align="left"], table[width="640"][cellpadding="7"]):has(a[href*="casino"])
nordfront.se##span:not(.post-content):has-text(/annons/i):upward(.post)
nordfront.se###campaign_area
nordichardware.se##span:has-text(/sponsrat/i):upward(.td_block_wrap)
nordichardware.se##.pspy_info, [class^="prisjakt-"]
nordichardware.se##.td-big-grid-post:has(a[href*="/sponsrat/"])
nordiskradio.se###cookieWindow
nordiskskog.se##.templateHelannonsBOX
norrahalland.se##.bannercontent
nouw.com##.washer.loaded.displayed
nouw.com##.badge:has-text(/annons/i):upward(li)
nyadagbladet.se##.third-col, article[class*="sponsrad"], div[id^="nyd-"], .below_header_front_page, div[data-aeon-news-trackbid="1"]
nyadagbladet.se##.widget_media_image:has-text(/annons/i)
nyadagbladet.se,ff.se,rocknytt.net,magasink.se,evergreengarden.se,butikstrender.se,mykitchenstories.se,transportnytt.se,inpress.com##.elementor-popup-modal
nyan.ax##.gdpr
nyan.ax##a[onclick*="banner"]
nyatider.nu##section.dce-visibility-event:has(a[href*="casino"])
nyatider.nu##.elementor-popup-modal:has(a[href="/integritetspolicy"])
nyatider.nu,autonytt.se##[href*="casino"][target]
nyfiknainvesterare.se##article.post:has-text(/annons från/i)
nyheter24.se##.breadtext_content.paywall_breadtext p:first-child::before
nyheter24.se##.lazyload_bar.show, .lazyload_outer.show, .sponsrat, .is_native, .sticky-scroll, .flow_ad
nyheteridag.se##article:has-text(/sponsrat innehåll/i)
nyheteridag.se##h2:has-text(/samarbetslänkar/i):upward(.article-inner)
nyheteridag.se##li:has(a[href*="kasino"], a[href*="casino"], a[href*="-slot-"])
nyheteridag.se##.widget.facebook, .content > div:not([class]) img, a[href*="www.casino"], a[href="/karnkraft.php"]
nyhetersto.se##.site-branding a ~ p, .wp-block-jetpack-slideshow
nyhetsbyranjarva.se##div[style="display: flex; justify-content: center; flex-direction: column; align-items: center;"]
nyhetsbyranjarva.se,nyan.ax,tv-kanal.se,golfguidenonline.se##.g
obosdamallsvenskan.se,elitettan.se##.rmss_ap-top-ad + .rmss_t-ap-grid-stripe:has(a[href*="svenskaspel"])
obosdamallsvenskan.se,elitettan.se##.rmss_module-sponsors, .rmss_ap-top-ad, .rmss_ad-panorama, .rmss_t-momenu__sponsors-area
obsid.se##a[href*="casino"]
offside.org###opab-modal, .opab-footer-offer
omnihalsa.com,skanesport.se,sportpanelen.se##.stream-item
omni.se,omniekonomi.se##div.group:has([class*="sponsoredcluster"])
omni.se,omniekonomi.se##.article--sponsored, .resource--sponsored, .component--sticky-sponsor-banner, .pre-banner, .banner--toppanorama, .banner--midpanorama, .group--banner
omni.se,omniekonomi.se##.header-banner--regular, .app-banner:style(--banner-offset: 0 !important;)
omni.se,omniekonomi.se##.resource--link:has(a[href*="article-ad-"])
omtanke.today##.featured
omvarlden.se,skolvarlden.se##.cookieControl
opulens.se##.mailpoet_form, #secondary
ordbokpro.se##+js(set, ab_disp, noopFunc)
ordfrontmagasin.se##.oc_cb_wrapper, .simple-image a:not([href^="/"]):not([href*="ordfrontmagasin.se"])
ordguru.se##.visible-lg, .hidden-lg
orebronyheter.com###top-wrapper
oru.se##.modal-cookieform
oru.se##.no-scroll:style(overflow: initial !important;)
oskarshamns-nytt.se##article.category-shoppingguide
oskarshamns-nytt.se##:is(.adsbygoogle, a[href*="casino"]):upward(.elementor-section)
osterbottenstidning.fi,sydin.fi,vasabladet.fi##.online-teaser--advertorial, .online-ad-container
padeldirekt.se##.article-row:has(.h-background--sponsored)
padeldirekt.se##.c-featured-article:has(a[href*="/sponsrat"])
padeldirekt.se##.text-center:has(div[id^="padeldirekt"])
padelfeber.se##.pfm-partners, .pff-partners, .c-widget-ad, .c-teaser--native, #toBanner
pakryss.se##div[id*="ad_banner"]
pilsner.nu##.overlay-loader
pilsner.nu##:is(.et_pb_fullwidth_image, .et_pb_image) a:not([href^="/"]):not([href*="pilsner.nu"]), .mctb-position-bottom
piraja.se###panoramaholder, #parallax, .cc-floating, a[href*="utm_medium=banner"]
piraja.se##:is(.intro, #hero, #featholder):has(.spons)
pirkt.se##aside#below-header, aside.sidebar-right img, aside.sidebar-left img, aside#above-main, aside#after-first-post, h1 + .wp-block-video, h2 + .wp-block-image img[src$=".gif"]
placera.se##.noMarginAd
placera.se##a:has-text(/^annons/i):upward(.section)
plastikoperationsforum.se,riksettan.net,automobil.se,endurobloggen.se,vibilagare.se,mopedgaraget.se,caroftheyear.se,klassiker.nu,alandsradio.ax,svjt.se,so-rummet.se###sliding-popup
playradio.se##.sidealtcol
podcasts.nu##.sponsor-list, .cookie-law-wrapper, .big-ad-placeholder, .affiliate-wrapper
poddtoppen.se##.txs-a
podtail.se##aside a[href*="utm_campaign"]
podtail.se##.item-list__item:has-text(/annons från/i)
pomu.se##[class^="Banner"]
poolforum.se##div.adfit, .cookie_notice, div[style^="width:100%;max-width: 728px;"] > div[align="center"], div[style^="width:100%;max-width: 728px;"] > br
popularastronomi.se##a.gofollow[data-track]:not([href*="www.popularastronomi.se"])
pressbladet.se,svenskpress.se,foretagsbladet.se,gestrikemagasinet.se,cfanytt.se,lasarnas.se,hembostad.nu,sportidrott.se,nojesmagasinet.nu,halsasverige.se,mandarinmedia.se##.isax, #cookiebar
pricerunner.se##span:has-text(/sponsra/i):upward(div[class$="Container-root"])
prisjakt.nu##.pjra-relative
proshop.se##body:style(background-image: none !important;)
proshop.se##.site-background-banner
pussad.se##html.g1-popup-visible:style(overflow: initial !important;)
pussad.se##.g1-popup-newsletter, .g1-slideup-wrap
quizza.nu###takeover
qx.se##.qxa-container
racenews.se###block-2
radiotreby.se##.mobileHide, .mobile-show
radio.se##:is(a[data-testid="region-tag"], a[data-testid^="taglist-item"]):style(background-image:none!important; background:rgb(2,114,140)!important;)
radio.se##:is(.md\:min-h-\[90px\], .lg\:min-h-\[250px\], .h-\[250px\], .justify-between.md\:mx-10):has(div[id^="RAD_D"], div[id^="RAD_M"])
ratsit.se##.promo
ravarumarknaden.se###header > div > div.last, #block-4, #mvp-leader-wrap
realtid.se##.link:has(.meta--add)
realtid.se##.realtid-add, .realtid-ad, .infinite-scroll.native-wrapper
recepten.se,foreca.se###topBanner
recept.se##div[class*="ad-wrapper"], button#cookiePreferences, .c-modal-backdrop--active
rejsa.nu###adsblock, #adsblockfoot, .fpright, div[onclick*="window.open"]
reseguiden.se##.adsbox-wrapper, .banner-xxl_panorama-container, .banner-top-container
restaurangvarlden.se##.banner-col, .alt-banner-col
res.se##.res-display
ridsport.se##.svrf__sticky-ad, .svrf-block__banner, .sv-cookie-consent-banner, .sp-banner-block, .sp-double-ad-block, .sp-head-sponsor-container, .sp-regular-sponsor-container
riktighockey.se###custom_html-2
rocknytt.net##[data-widget_type*="bnnrwidgets"], a[href*="/annons/"], div[data-widget_type="image.default"] a[target="_blank"]
rodeo.net##article[data-section="allmänt"]
runnersworld.se##.post-card-sponsored, .modal-plus, .modal-backdrop
runnersworld.se,motormagasinet.se,dagenshandel.se,food-supply.se,plastnet.se,habit.se,woodnet.se,foodnet.se,transportnet.se,processnet.se,packnet.se,verkstaderna.se,medtechmagazine.se,recyclingnet.se,rt-forum.se,uochd.se,lifesciencesweden.se,fri-kopenskap.se,cleannet.se,metal-supply.se,framtidensbygg.se,entreprenad.com,branschstegen.se,skogsforum.se,bio.se##.modal-open:style(overflow:initial!important)
runnersworld.se,utsidan.se,hockeymagasinet.com,driva-eget.se,foretagande.se,revisionsvarlden.se,travelnews.se,mittforetag.com##.sponsored
sakochliv.se##+js(acs, checkCampaignCookie)
sakochliv.se##.cookie-disclaimer-wrap, .type-promo, .sector-annons
samfalligheterna.se##.tdm-popup-modal-wrap
samfalligheterna.se##.tds-locked-content:style(display:unset!important;)
samfalligheterna.se##.tds-locked-content[hidden]:remove-attr(hidden)
samfalligheterna.se##.td-cpt-post:has(a[href*="/sponsra"])
samfalligheterna.se##.td_block_wrap:has-text(Annons)
samnytt.se,samnytt.nu##a[href*="casino"], a[target="_blank"] img:not([class^="tweet-"]), a img[src^="/butik"]
samnytt.se,samnytt.nu##.sticky > div:has(img[src^="/butik"])
sanghafte.se##.widget_cooperations
sanghafte.se##.wp-show-posts-single:has(a[href*="casino"], a[href*="kasino"], a[href*="betting"])
sbf.se##.sv-cookie-consent-banner, .hiq-partners-banner
scanaktier.se###overlay-black
schack.se##.schac-widget
schoolido.se##.so-cookie__area
screen-marknaden.se##.fo-banner, .fp-banner
sdhl.se,ssl.se,storvretaibk.se##.rmss_module-block-linked_image, a[href*="svenskaspel.se"]
sdhl.se,ssl.se,storvretaibk.se,obosdamallsvenskan.se,elitettan.se,ifiske.se##.cc_banner-wrapper
selectAdvertiserElement$domain=bebisvarlden.se
senses.se##aside:has-text(Annonser:)
senses.se##a[href*="casino"], a[href*="spelsajt"], a[href*="betting"]
sexpacket.se##+js(aeld, /contextmenu|cut|copy|paste/)
sexpacket.se##.info_cookies
se.azrhymes.com##div[id^="azrhymes_com_between_content"]
shoegazing.se###main-sidebar .widget_media_image, #post-sidebar .widget_media_image, #content > .code-block
shortcut.se##div[class^="baner"], a[target="_blank"] img
shortcut.se##.category-tag:has-text(/annons/i):upward(.ArticleListItem)
sidebanner$image,domain=samnytt.se|samnytt.nu
signprint.se##.topbanner
signprint.se##p:has-text(SPONSR):upward(.elementor-widget-jet-listing-grid)
siljannews.se##article:has(a[href^="/annons"])
siljannews.se##a[target="_blank"]:upward(2)
siljannews.se##h3:has-text(/Annons/i) + div
siljannews.se##p > a:not([href*="siljannews.se"]):not([href^="/"]) img
siljanskok.se##a[target="_blank"][rel="nofollow"]:upward(1)
siljanskok.se###app > div[data-reactroot] > div:first-child:has(a[target])
sillyseason.se##li:has(a[href*=".se/odds/"], a[href*="/betting/"], a[href*="kasino"], a[href*="/promomen/"])
sillyseason.se##strong:has-text(casino):upward(li.sidebar-widget)
sillyseason.se###text-41, #leader-wrapper, a[href^="/till/"][target="_blank"]
siriusbandy.se,vetlandabk.se##[id$="-ad"]
si.se,sweden.se###cookie-manager
sjofartstidningen.se###newsletter-overlay, #newsletter-modal
sjofart.ax##section.huvudsektion:style(margin-top:unset!important)
sjofart.ax##:is(.sjofa-top-takeover, .sjofa-artikel-pano):upward(section)
sjostadsbladet.se##a.td_single_image_bg, span.td_single_image_bg[data-img-url*="Annons"]
sjostadsbladet.se##.td-category-pos-:has(a[href*="casino"])
skaneplus.se##div[style="padding-top:0px;padding-right:0px;padding-bottom:0px;padding-left:0px;flex-basis:50%"]:has(a:not([href*="skaneplus.se"]):not([href^="/"]) > img)
skanesport.se###black-studio-tinymce-3, .menu-item a[target="_blank"], .footer-widgets
skargarden.se##article:has([title^="Annons"], a[href*="/annons"])
skargarden.se###topbanner, #mittbanner, #topbannerm, #mittbannerm
skidspar.se###videoad
skillingaryd.nu,xn--vrnamo-bua.nu###more-banners
skk.se###cookie-button-banner, .campaigns, [id*="GlobalCampaigns"]
skogen.se##.jobslider.up
skogsforum.se##.masthead, .col-right, a[href^="https://goo.gl/"], a[href*="//bit.ly/"], a[target="_blank"][onclick], #ap1, .modal, .modal-backdrop
skogssallskapet.se,formas.se,rf.se##body:style(overflow:initial!important; position:initial!important;)
skogssallskapet.se,formas.se,rf.se##.env-modal-dialog--show, .env-modal-dialog__backdrop
skolfamiljen.se##.right-sidebar aside[id^="block"], .right-sidebar aside[id^="adguru"]
skolporten.se##.article-short:has(a[href*="/sponsrat-innehall"])
skrattnet.se##.region-sidebar-second
skrattsajten.com,norpan.se##.cookieScript
skrattsajten.com,norpan.se##+js(acs, $, e.preventDefault)
skyltat.se##.sidebar
skyscanner.se###modal-container, div[data-testid="advert-card-gam"]
smartsenior.se##.ss-modal, .modal-mobile-app
snowmobile.se##div[itemtype="https://schema.org/WPAdBlock"], .bs-wrap-gdpr-law
sokbat.se##a[target="_blank"][onclick]
sonicmagazine.com,ratsit.se,dagensinfrastruktur.se,nyaprojekt.se,nordiskaprojekt.se,svenskbyggtidning.se,grontsamhallsbyggande.se##[class^="ad-"]
so-rummet.se##h3:has-text(/annonser/i):upward(.view-nya-lankar-front)
so-rummet.se##.article-list:has(.sponsrad-over)
so-rummet.se##.block-rr
so-rummet.se##.link-list-item:has(img[src*="sponsrad"])
spanaren.se,horisontmagasin.se,shoegazing.se##.textwidget a[target*="blank"] img
spelagratis.se##.sidebar-right, .ad_header + p
spelhubben.se##html, .unselectable:style(-moz-user-select:initial!important; -webkit-user-select:initial!important; -webkit-touch-callout:initial!important; user-select:initial!important; -webkit-tap-highlight-color:initial!important; cursor:initial!important;)
spelhubben.se###slideout
spelhubben.se,husbilsplats.se##+js(acs, document.oncontextmenu)
spelochfilm.se##a[href*="casino"]:upward(.mh-posts-stacked-wrap)
spelochfilm.se##.mh-sidebar .textwidget
spelo.se,lokalguiden.se,svenskverkstad.se##.banner-container
sponsor$image,domain=obosdamallsvenskan.se|elitettan.se
sportal.se##.cookie-div, a[href$="/banner/"]
sportbilen.se###text-4
sportbladetplay.se##body.dimmed:style(overflow:unset!important)
sportbladetplay.se##.ui.page.dimmer:has(div[class^="CookieConsentPopup"])
sportbloggare.com##div.section-body-plus:has-text(/bonus|casino/i)
sportbloggare.com##.container:has-text(Senaste nyheterna om spelbolag:)
sportbloggare.com##.partners-box, .cube-bonus-list, .section-featured-links-column, .section-bonus-list, a[href="https://sportbloggare.com/casino-bonus"], a[href="https://sportbloggare.com/bettingsidor"], a[href="https://sportbloggare.com/betting-bonus"]
sportbloggare.com##.section-body-plus .body-block:has(a[href*="betting"])
sporthalsa.se##a[href*="/annonsering"]
sporthalsa.se##h4:has-text(veckans produkt):upward(3)
sporthalsa.se##.header_top, #media_image-2, #text-6, article[class*="veckans-produkt"]
sportlovin.se##.visible-xs, .visible-lg
sportpanelen.se##.textwidget:has(a[href*="casino"])
sportsnews.se,xn--sporthnt-5za.se###secondary:has(a[href*="casino"])
sporttv.nu##a[onclick*="bannerClick"], #linkus, .details-bet-banner
spray.se##body:style(-webkit-user-select: text !important; user-select: text !important;)
spray.se##section[class*="casino"], a[href*="casino"]
spray.se##+js(set, googletag, 1)
spray.se,vinochmatguiden.se##+js(set, window.WURFL, 1)
stallet.se##.pnlAdTop
stallet.se##+js(alert-buster)
startaochdriva.se##.banner-right, .banner-left, .wpb_single_image a[target="_blank"], .tdm-popup-modal-wrap
startaochdriva.se##:is(.latest-post, .td-cpt-post):has(a[href*="/sponsrat"])
stegforhalsa.se##[class*="jsx-"][style*="position: sticky"], .bc--grey-neutral-50[style^="min-height"]
stoppapressarna.se##.premium-page-ad, .footer-banner-wrapper, div[id^="stopp-"]
storyhouseegmont.se##body.freeze-scroll:remove-class(freeze-scroll)
storyhouseegmont.se##div[class^="Navigation__Overlay"]
streamio.com,nyan.ax,spelhubben.se,illvet.se,varldenshistoria.se##+js(aeld, contextmenu)
surfa.se##div[class*="-promo"], div[class*="prisjakt-"]
surfa.se,teknikfreak.se###loader-wrapper
svampguiden.com##.label-sponsor:upward(.panel)
svartgul.se##li.embedded
svartgul.se,eventeffect.se,executiveeffect.se,saleseffect.se###panorama
svd.se##article:has(div[class^="NativeBarWrapper"])
svd.se##body:style(visibility:visible!important;)
svd.se###mega-ad-wrapper, div[class*="advertory"], div[data-custom-ad-handled="true"], span[data-id="bottom-sticker-offer"], div[data-context-pageview*="native-svd"]
svd.se,chef.se,vvsforum.se,elinstallatoren.se,arkitekten.se,natursidan.se,svenskfarmaci.se,da.se,frisor.se##.Ad
svenskafans.com##.puff__ad-heading, ad-skyscraper__wrapper, iframe[title*="Bet 365"]
svenskahousegruppen.se##body.modal-open:style(overflow:initial!important)
svenskahousegruppen.se###eprivacyModal, .modal-backdrop
svenskalag.se##.cookie-overlay, .cookie-box
svenskarnaochinternet.se,internetstiftelsen.se###newsletter-sliding
svenskbyggtidning.se,nyhetersto.se,bussmagasinet.se,brollopsmagasinet.se,borattforum.se,globalpolitics.se,batliv.se,em-fotboll.se,elinor.se,fotbollsresultat.com,automation.se,vm-fotboll.se,husbyggaren.se,vildmarken.se,fisheco.se,nyhetsbyranjarva.se,it-finans.se,it-halsa.se,it-kanalen.se,it-pedagogen.se,it-retail.se,it-hallbarhet.se,battregolf.se,sporthalsa.se,revisionsvarlden.se##a.gofollow[data-track]
svenskelitfotboll.se##custom-ad, sponsors
svenskelitfotboll.se##.image-block:has(a[class*="sponsor"])
svenskfarmaci.se##.Dialog[data-dialog-skip-auto-open-for-utm-source-value="Newsletter"]
svenskfotboll.se##.news-multi-link--sponsor
svenskgolf.se##.highlight:has(.partnerLabel)
svenskgolf.se,husohem.se,tidningenhalsa.se,vagabond.se,praktisktbatagande.se,akaskidor.se,utemagasinet.se,sportfack.se##.partnerCard, .partnerContent, .entry-content figure.wp-block-image, .category-partner, .ams-playad-injected
svenskhistoria.se##.widget_et_ads, .module-etads, #text-13, #block-4, a[target="_blank"][rel="noopener noreferrer"], a > img[width="300"][height="250"], a > img[width="800"][height="175"], a[href*="casino"], a[href*="poker"], a[href*="kasino"], a img[width="1000"][height="300"]
svenskhistoria.se##.widget_text:has(a[href*="casino"])
svenskjakt.se###survey-dialog
svensktgolfforum.se##[data-ad-id], .darkenwrapper
svensktidskrift.se###bannercolumn, img[title^="Annons"]
svensktidskrift.se##.tf_svg_lazy:style(transition:none!important; filter:none!important; transform:none!important;)
svenskverkstad.se##app-exposure-small
svenskverkstad.se##svv-short-news-widget:has(.native-news-link)
svenskverkstad.se##svv-wide-news-widget:has(.annons)
sverigesindustri.se##.article-item:has(.article-label--sponsored, .article-item--sponsored)
sverigesnatur.org##div[id^="sverigesNaturPopup"]
sverigespringer.se##.cd-card-bar:has-text(/annons/i):upward(.cd-sidebar-item, .cd-news-card)
sverigespringer.se##.cd-desktop-banner
sverige.nu##a[href*="casino"]
sweclockers.com##div[class^="card-info"]:has-text(/spons/i):upward(.card)
sweclockers.com###prisjakt-popular, .ad:not(.adPanorama), .adForumSticker, .dark-mode__sponsor
sweclockers.com##.ad.adPanorama:style(height:100px!important; position:absolute!important;)
sweclockers.com##.bbSize:has-text(Sponsormeddelande):upward(.bbRelatedBox)
swedroid.se##a[target="_blank"]:upward(li.Notice):remove()
swedroid.se##div[id$="_ad"], div[id$="_ad_mobile"], .externalTopMobile, #externalTopMobile, .externalBottomMobile, a[href^="//www.prisjakt.nu/produkt"], #nativendo-mainfeed + aside > .article, .article-footer > h3, .article-footer > .aeChart, #newExternal
swedroid.se##span:has-text(/sponsr/i):upward(.article)
swedroid.se##+js(set, checkAdsBlocked, noopFunc)
swedroid.se##.mostReadMobile:has-text(/annons/i)
swedroid.se##.puff:has(script[src*="lwadm.com"])
swehockey.se##[class*="-reklam"], .sif-sponsorer, .teaserblock, .commonblock a:not([href^="/"], [href*="/swehockey.se"])
sydasien.se##.thb-cookie-bar
sydnarkenytt.se##.toppbanner-outer, .reklamplats_hspalt, .egenbanner
synonymer.se##+js(cookie-remover, /^ev_did|ev_sid/)
synonymer.se##.create-account-banner, .buy-premium-banner, div[class*="pb-"] > div.text-center
tabyallehanda.se##p:has-text(ANNONS)
tabyallehanda.se##section[id^="Panorama"]
tandlakartidningen.se##[class^="ad-container"], [class^="adbox-single"], div[id^="takeover-"]
tasteline.com##.article.related > a[href*="&utm"][target="_blank"]
tasteline.com##.popup-overlay
tasteline.com##.popup:style(overflow: auto !important;)
techmag.se##div[style="clear:both;float:left;width:100%;margin:0 0 20px 0;"]:has(.contentadx)
techmag.se##.popup-overlay, div[id^="techmag_com"], .contentadx
techmag.se##.widget_codewidget:has(div[id^="techmag_com"])
teknifik.se##.post:has(.sponsor)
teknikguiden.se##:is(.vce-sticky, .vce-content-bottom):has(a[target])
tekniknytt.se##.label:has-text(/samarbete|annons|reklam|presenteras av/i):upward(a)
tekniknytt.se##:is(.article_widget_preview, .article_widget_listing):has(a[href*="casino"], a[href*="kasino"])
tekniknytt.se##:is(.top-news, .big_article):has(img[src*="casino"], img[src*="surfeo"])
tekniknytt.se##[onclick^="ga("]:remove-attr(onclick)
tekniksmart.se##center:has-text(/annons/i):upward(1)
tekniksmart.se##.code-block, main > div:last-child:not(:only-child), #uid_08313ba73, #uid_ab3738b5a, .jeg_header_wrapper .jeg_midbar
tekniksmart.se##.wpb_row:has(a[href*="casino"])
teknikveckan.se##.pill:has-text(/spons/i):upward(.grid-item, .pinned, .articleFlow-item)
teknikveckan.se,di.se,dn.se,skillingaryd.nu,xn--vrnamo-bua.nu,vardfokus.se,kamerabild.se,tripadvisor.se,swedroid.se,bettingstugan.se,expressen.se,dagensopinion.se,driva-eget.se,bioenergitidningen.se,ifokus.se,padelfeber.se,sv.picmix.com,ifragasatt.se,ehandel.se,jaktojagare.se,sportbloggare.com,bovision.se,familjeliv.se,tidningenridsport.se,golflivet.se,vemringde.se,brollopstorget.se,fastighetsvarlden.se,borskollen.se,aktiespararna.se,receptfavoriter.se,tyda.se,mittforetag.com##.ad
teknologiexperten.se##a:has(img[src*=".se-www"]), a[href*="casino"]
temaarkiv.se##.md\:mt-\[100px\]:has(script[data-adfscript])
temadagar.se##+js(acs, chp_adblock_browser)
temadagar.se##.ez-sidebar-wall
temperatur.nu##.holidAds:upward(1)
tennisportalen.se##h4:has-text(/spons/i):upward(.td-pb-row [class*="td-pb-span"])
testfakta.se##.row-uppdragstest
thatsup.se##+js(set, canShowAds, true)
thelocal.se##.ad-container-section, .article-sponsored, div[data-hasbanner="yes"]
thelocal.se##.ra-widget-article-tag:has-text(/partner/i):upward(.ra-widget-panel)
thelocal.se##.single-article-related.single-article-related-short:style(height:unset!important; overflow:unset!important;)
thelocal.se##.single-article-related.single-article-related-short::after:style(background:unset!important;)
thepattayanews.se##a.td_single_image_bg:not([href*="thepattayanews.se"]), #tnp-modal
thorengruppen.se,utslappsratt.se,heleneholmsif.se,trafikskola.se,melodifestivalklubben.se,morotsliv.com##+js(set, em_track_user, false)
thorengruppen.se,utslappsratt.se,heleneholmsif.se,trafikskola.se,melodifestivalklubben.se,morotsliv.com##+js(set, exactmetrics_frontend, undefined)
tidningenbalans.se##div[style*="z-index: 999; background-color: rgba(0, 0, 0, 0.5)"], .bg-grey.hideOnPrint, .bg-adYellow
tidningenbalans.se##p:has-text(/i annonssamarbete med/i):upward(.flex.overflow-hidden)
tidningendacksnack.se##.ann-puff
tidningenglobal.se,tidningensyre.se,landetsfria.nu,fempers.se##.revive-box
tidningennara.se,odenochaventyr.se##.cookie-bar
tidningenridsport.se##body:remove-class(cli-barmodal-open)
tidningenridsport.se##.entry-content:style(display: initial !important;)
tidningenridsport.se##.subscribe_now_popup, .type-native, #captive, .hldr_takeover_nl.show, .hldr_takeover
tidningenskriva.se##section.widget_text:has(div[id^="ad-"])
tidningen.djurskyddet.se##.ai-track
tidningen.nu##span:has-text(/^Annons$/):upward(1) + .textwidget
tidningen.se##.sidebar .widget_widget_code, .casino
tillnyktrad.se,webhallen.com##.cookie-consent
tittapavideon.se##.adv
tlnt.se##div[id^="ad-block"]
tlnt.se##.fakta-list:has-text(/annons/i)
tonyhatefnejad.se,lyckasmedbakning.nu,pinkprogramming.se,brl.se,naturnaraskogsbruk.se##.preloader
totallyorebro.se,totallystockholm.se##div.tot-content-preview-container-small[style*="border-top:4px solid #ffb200;"], .content-overlay--black, a[href*="casino"], a[href*="/sponsrat/"], a[href*="/sponsrat/"] + p.tot-content-preview--meta, .newaddiv, .tot-sidebar
totallyorebro.se,totallystockholm.se##[class*="tot-content-preview-container"]:has(a[href*="casino"], a[href*="kasino"], a[href*="betting"], a[href*="spel"]):remove()
trafikradion.com##.right
tranakampsport.se##.w-dyn-item:has(.sponsrad-artikel-wrapper:not(.w-condition-invisible))
traning40plus.se##[id^="bunyad"]
travelnews.se##.bottom-bar--animate-in, #job_ads_scroller, .header_banner
travnet.se##.hidden:has(div[id^="travnet_"])
travronden.se##a[href*="/sponsrat/"]
travronden.se##div:matches-css(visibility: hidden):has-text(ANNONS)
travsport.se,gavletravet.se##.banner-component, .partners, .cookie-meddelande
trendenser.se##strong:has-text(/reklam/i):upward(.post_feed_post)
trendenser.se##.featured-post:has(a[href*="/category/reklam"], a[href*="/category/annons"])
trendenser.se##.post_feed_post:has(.sponsor-info)
tripadvisor.se##a:has-text(/Sponsrat av|i samarbete med/i)
tripadvisor.se##[class$="banner_ad"]
turismnytt.se##.site-wrap > .row > .col-sm-3
turistmal.se###col_right
tv4play.se,tv4.se,fotbollskanalen.se,koket.se##button:has-text(Besök annonsör)
tv4play.se,tv4.se,fotbollskanalen.se,koket.se##+js(json-prune-fetch-response, playbackItem.isStitched, , propsToMatch, url:a2d.tv/play)
tv4play.se,tv4.se,fotbollskanalen.se,koket.se##+js(xml-prune, Ad, , /fwmrm.net\/ad\/g/)
tv4play.se,tv4.se,fotbollskanalen.se,koket.se##.avod-web-player-pause:style(background-color:transparent!important;)
tv4.se##.maxetise
tv24.se##li[id^="infeed"]
tvmatchen.nu##.bet365, .panorama-wrapper, .tvg-manager-box, .tv102945, .tv102987, #event_banner, .go-to-partner, .odds, #text-13
tvprogram.se##.backdrop, .fcb
tv.nu##a[href*="adform.net"], .ad-fullscreenWallpaper__container
tv.nu##body:remove-class(takeover-loading)
tv.nu###tv-schedule section:has-text(ANNONS)
tyda.se##.frontpage_article:has(a[href*="casino"], a[href*="kasino"], a[href*="betting"], img[data-cfsrc*="Sponsra"])
typkanske.se##.adbar
underbaraclaras.se##.jet-listing-dynamic-field__content:has-text(/annonssamarbete|reklamsamarbete/i):upward(.jet-listing-grid__item)
undertian.com###cookieNotification, .gad, div[style^="font-size:11px; margin-left"], div[style^="font-size:11px; margin-left"] + div[style]
undervarttak.se##.middle-banner
ungdomsfotboll.se##div[id^="ungdo-"]
universitetslararen.se##div[id^="unive-"]
upphandling24.se##aside .textwidget:has-text(ANNONS)
upphandling24.se##.type-partnerartikel
uppsalanyheter.se###banner-top-block
uppsatser.se##.results li[style^="margin"]:not(.result)
upptack-sverige.se##.front-cta:has-text(/sponsrat innehåll/i)
usabil.nu##.image-post-link[target]
utm_$document,removeparam=/^utm_/,domain=tv.nu|booli.se|expressen.se|aftonbladet.se|bostad.blocket.se|dagensps.se|prisjakt.nu|vinborsen.se
utsidan.se##.clamzone
utsidan.se##.betart-marker:matches-css(after, content: /Annons/i):upward(.documentpush-group)
vackertvader.se##div[class^="ad-300x250"], div[class^="ad_300x250"]
vackertvader.se,tidningenskriva.se,veckansnyheter.se,eventeffect.se,executiveeffect.se,saleseffect.se##.cc-window
vadvivet.se##html.has-intro-popup:remove-class(has-intro-popup)
vadvivet.se##html.show-intro-popup:remove-class(show-intro-popup)
vadvivet.se##.intro-popup
vagabond.se##.latest-article-native
varden.se##app-native-puff, .header-top-banners
varden.se##.carousel-slide:has(.sponsored-label)
vardfokus.se,tidningenridsport.se##.cli-modal-backdrop
vardpraktikan.se###nyhetsbrev
varldenshaftigaste.se##[id*="annons"], #getFixed
varmepumpsforum.com##.stopjump
varmepumpsforum.com##a[target]:upward(.frontlinks tr)
varmepumpsforum.com,poolforum.se,lindenytt.com,autopower.se,arjeplognytt.se,jaktsidan.se##a[target="_blank"] img[alt]
vartgoteborg.se##div[class^="Popup"], div[class^="CookieBanner"]
varvat.se##.wpb_single_image a[target], .gp-footer-2
vasterastidning.se##article[data-section="nativeannons"]
vasterastidning.se##.row:has(a[href*="casino.se"])
vasterastidning.se##:is(h2, h5, .kicker):has-text(ANNONS):upward(article, div.row)
veckansmiddag.com###load
veckorevyn.com##.annons-block
veckorevyn.com##.g1-mosaic-item:has(.category-annonssamarbete)
veterinarmagazinet.se##.nyhet-ad
vf.se,hjotidning.se,kt.se,kt-kuriren.se,sla.se,mariestadstidningen.se,filipstadstidning.se,fryksdalsbygden.se,nwt.se,arvikanyheter.se,nkp.se,saffletidningen.se,provinstidningen.se,dalslanningen.se,nlt.se,skaraborgsbygden.se##[data-testid="ad-area"], footer + div.shadow-lg.fixed
vibilagare.se##a[href^="/partnermaterial/"]
viivilla.se###rich-media-wrapper
viivilla.se##.teaser:has(.teaser__native-marker)
vilaser.se##.Internal-ad
villalivet.se##.mtsnb, .villalivet-target, a[href*="/sponsrat-innehall/"], div[data-td-block-uid="tdi_85"], a[href*="utm_campaign"][target="_blank"], div[data-td-block-uid="tdi_87"]
villalivet.se##:is(a, span):has-text(/sponsr/i):upward(3)
villatidningen.se##.wppsac-post-carousel:has(a[href*="/spons"])
vimedbarn.se##button:has-text(/annons/i):upward(.owl-item):remove()
vimedbarn.se##.annonsinlagg, .annonsen
vinbanken.se##.fancybox-lock:style(overflow-y: auto !important;)
vinbanken.se##.push-to-newsletter, .fancybox-overlay
vinbanken.se##.top-add, .sidebar-adds, .spons-content
vinliv.se##.product_banner_wrapper
vinochmatguiden.se##.popup_missa-inget
viseniorer.se##.topheaderinfo
viseniorer.se##.leftinfo:has-text(/Externa artiklar:|Länktips:/)
vi.se##body.cookie-modal-open:style(overflow:unset!important;)
vi.se###westander-cookie-dialog, .Cookie-consent__backdrop
vk.se,folkbladet.nu,nordsverige.se,mellanbygden.nu,vasterbottningen.se,lokaltidningen.nu##.vkmui-Text--grey, [class^="adContainer"], div[class^="bordersAndShadows"] > div[style^="min-height"]:only-child, div[data-track-id="family.Familjeannonser"], div[class*="adElement"]
vmj.se##.sidebox:has-text(/Externa länkar|Artiklar/)
vmj.se,danskaspraket.se,digitalavykort.se##.topdiv
vmj.se,danskaspraket.se,digitalavykort.se,viseniorer.se##.cc-cookies
vm-fotboll.se##a[href*="/go/"][target], .category-kampanjer
vm-fotboll.se##.fusion-text:has-text(Online casino)
voister.se##div[class^="articles_articleBrief"]:has(div[class*="articles_campaign"])
voodoofilm.org##.card-header:has-text(Annons):upward(.card)
voodoofilm.org##.content-news:has(span[id*="Sponsored"])
voodoofilm.org##.page-panorama
vovve.net##span:has-text(/^i samarbete med/i):upward(2)
vovve.net###sticky_ad, div[style*="ad_hor.gif"], a[href*="casino"], a[href*="kasyno"], a[href*="betting"], a[href*="spelsajter.eu"], a[href*="spelsidor.org"], a[href*="oddsgurun.com"], a[href*="betsidor"], a[href*="välkomstbonusar"]
webbjobb.io##.cookie
webbkameror.se###cookiescript_injected
webbkryss.nu##.skyad-wrapper
webb-tv.nu##[id^="adservice"]
webhallen.com##.takeover-link
whowhatwear.co.uk#@#a[href*="/click.linksynergy"] img
www.aftonbladet.se##+js(nostif, TAKEOVER)
www.expressen.se##+js(set, detect, noopFunc)
www.expressen.se##.video-player:remove-attr(data-ad-config)
www.expressen.se,di.se##+js(aeld, contextmenu, .disabled)
xn--lnforum-exa.se##.LFRBox
yogafordig.nu##.popup-large, .popup-bottom, .square-banner-wrapper
ysektionen.se##.yweb-news-paper-banner
zeinaskitchen.se,trafiksakerhet.se,boktugg.se,lakartidningen.se,villalivet.se,matsafari.nu,forexgruppen.se,fastighetsvarlden.se##+js(acs, monsterinsights_frontend)
zeinaskitchen.se,trafiksakerhet.se,boktugg.se,lakartidningen.se,villalivet.se,matsafari.nu,forexgruppen.se,fastighetsvarlden.se##+js(set, mi_track_user, false)
zeromagazine.nu##div[id^="ads"]
##.lazyb.panorama
##adsaga-banner
##article.NativeTeaser
##article.annons
##article.sponsrad
##article.article-list-item--sponsored-post
##article.article-sponsored
##article.article--sponsored
##article.category-partnerartikel
##article.category-promotion
##article.category-reklam
##article.category-samarbete
##article.category-samarbete-sponsrat
##article.category-samarbete-sponsrat-inlagg
##article.sponsrat-inlagg
##article.tag-adtraction
##article.tag-annons
##article.type-partnerartikel
##article[data-section="sponsrad"]
##aside.ad-container
##a#top-banner.banner-holder
##a.adv-link
##a.card.-sponsored
##a.is-native-ad
##a[data-bid="1"][href*="/linkout"]
##a[href$=".se/go/betsafe"]
##a[href*="casinopro.se"][target="_blank"]
##a[href*="cyberbetpromo.net/click"][target="_blank"]
##a[href*="doktor-se.onelink.me"]
##a[href*="tradedoubler.com/click?"]
##a[href*="utm_content=banner"] img
##a[href*="www.bildelaronline24.se"][target="_blank"]
##a[href*="www.reservdelar24.se"][target="_blank"]
##a[href*="/annonsartiklar/"]
##a[href*="/banner/klick/"] img
##a[href*="/click.adrecord"] img
##a[href*="/click.linksynergy"] img
##a[href*="/cvasino.se/"] img
##a[href*="/delivery.adnuntius.com"]
##a[href^="https://www.adsettings.com/scripts/reg_click."]
##a[href^="/banner/click/"] img
##a[id^="adBanner"][target="_blank"]
##a[onclick*="AdRotatePro"]
##a[onclick*="artikelbanner"]
##a[title="LeoVegas"]
##body[data-site-namespace="tailsweep"] #premiumAdWrapper
##div.NativeAd
##div.adDivLeft
##div.adDivRight
##div.adLinkInner
##div.adSidebar
##div.ad.container
##div.ad.panorama
##div.annonsbox
##div.bbPrisjakt
##div.holidAds
##div.outsideAdsWrapper
##div.panoramaAd
##div.toppannons
##div.wppasrotate
##div#ads-panorama
##div#ads_column
##div#ad_global_below_navbar
##div#annons_topp
##div#banner_right
##div#block-adreviveheader
##div#custom_ads_wrapper
##div#facebook-popup
##div#mega-ad-content
##div#outerAd
##div#outside-ads
##div#panoramaad
##div#panorama_ad
##div#reklam
##div#rich-media-ads
##div#schibsted-data-controller-sticky
##div#snow-container[style*="z-index: 999999"]
##div#toppannons
##div#topreklam
##div#zox-lead-bot
##div.CMACG_AdChangerWidget
##div.Container--ad
##div.External-ad
##div.adform-container
##div.adnuntius-ad
##div.ads-sticky-container
##div.adtech_slot
##div.advads-background
##div.ad-after-header
##div.ad-after-post
##div.ad-component
##div.ad-container-lg
##div.ad-panorama_dynamic-wrapper
##div.ad-toppbanner
##div.after-article-ad
##div.annons-yta
##div.article-ad-container
##div.ashe-preloader-wrap
##div.bam-ad-wrapper
##div.banner-size.proad
##div.before-article-ad
##div.better-ads-listitemad
##div.big-desktop-ads
##div.block-bean-header-banner
##div.borka-ad
##div.box--squareAd
##div.brix-ads-by-posttype
##div.bsa_pro_ajax_load
##div.column-article.tag-annons
##div.comment-ad_wrapper
##div.content-center-ad
##div.content_ad_top
##div.elementor-widget-wp-widget-adrotate_widgets
##div.elementor-widget-wp-widget-advads_ad_widget
##div.feed_ad
##div.fs-holid-live-widescreen
##div.helsida-ad
##div.inner_advertisement
##div.in-post-ad-wrap
##div.jeg_ad
##div.js-top-banner-container
##div.landscape-ad-space
##div.leeads-wrapper-desktop
##div.link-ads
##div.l-footer__adtext
##div.maaw-ad-slots
##div.medium-ad
##div.mgp-ads
##div.mosaico-ad
##div.navbar-ad-section
##div.novashare-buttons
##div.o-indenter--ad
##div.panorama-ad
##div.panorama-ad-standard
##div.partnership-ads
##div.phpbb-ads-center
##div.prebid-ad-slot
##div.sb-egmont-plugin
##div.schibsted-info-sticky
##div.sch-datacontroller--footer
##div.sch-datacontroller--subheader
##div.sgm-ad
##div.sgm-header-start-ad
##div.sgm-large-ad
##div.sidebar-annons
##div.sidebar-item .banner-box
##div.strossle-widget
##div.td-a-rec img
##div.td-banner-bg
##div.topmost-banner
##div.view-annons-banner
##div.vue-ad-wrapper
##div.widget_widget_dfp
##div[class$="popup-and-layer-ads"]
##div[class*="ai-viewport"][data-insertion-position]
##div[class*="bsaProContainer"]
##div[class^="borka-insider"]
##div[class^="borka-panorama"]
##div[class^="borka-widescreen"]
##div[class^="holid_desktop"]
##div[data-losjs^="borka-insider"]
##div[data-losjs^="borka-panorama"]
##div[data-losjs^="borka-widescreen"]
##div[id^="ad_insider"]
##div[id^="borka-insider"]
##div[id^="borka-panorama"]
##div[id^="borka-widescreen"]
##div[id^="matchads-"]
##footer .sponsors-area
##iframe#compricer_iframe
##img[alt="Leovegas"]
##img[alt="Spela på Betsson"]
##img[src*="/track.adtraction"]
##ins[data-revive-zoneid]
##td#reklam
##ul.adsmodern
###RightOuterBannerDiv
###advisa-iframe
###ad-fullscreen:not(body):not(html)
###ad-mega-container:not(body):not(html)
###ad-wallpaper:not(body):not(html)
###ad_topScroller:not(body):not(html)
###annons_head
###bottomAnnonsBar
###div-leeadsFullpageAd
###leeads-panorama-container
###strossle-below-article-thumbnails
###topBannerAds
##.Teaser--nativeAd:not(body):not(html)
##.adContainer:not(body):not(html)
##.adrotate-group:not(body):not(html)
##.adtoma_container:not(body):not(html)
##.adtrue-holder:not(body):not(html)
##.ad-rotator:not(body):not(html)
##.ad-single-news:not(body):not(html)
##.ad_container_bottom:not(body):not(html)
##.annonseArticle:not(body):not(html)
##.annons_mitten:not(body):not(html)
##.annons_panorama:not(body):not(html)
##.bannerclick:not(body):not(html)
##.b-ad__wrapper:not(body):not(html)
##.carrie-ad-block:not(body):not(html)
##.casino-ad:not(body):not(html)
##.category-annonssamarbete:not(body):not(html)
##.category-annons:not(body):not(html)
##.category-om-samarbeten:not(body):not(html)
##.category-samarbeten:not(body):not(html)
##.category-sponsrade-inlagg:not(body):not(html)
##.category-sponsrade-reklaminlagg:not(body):not(html)
##.category-sponsrad-artikel:not(body):not(html)
##.category-sponsrad:not(body):not(html)
##.category-sponsrat-content:not(body):not(html)
##.category-sponsrat-inlagg:not(body):not(html)
##.category-sponsrat-innehall:not(body):not(html)
##.category-sponsrat:not(body):not(html)
##.component-matchAds:not(body):not(html)
##.component-matchAds__content:not(body):not(html)
##.c-ad-wrapper:not(body):not(html)
##.c-ad__floating:not(body):not(html)
##.c-dfp_ads:not(body):not(html)
##.c-post--native-ad:not(body):not(html)
##.dfp-ad-widget-class:not(body):not(html)
##.dj-ad-size:not(body):not(html)
##.esmg-hb-slot:not(body):not(html)
##.favethemes-content-ad-bottom:not(body):not(html)
##.favethemes-content-ad-inline:not(body):not(html)
##.favethemes-content-ad-top:not(body):not(html)
##.footer-ad-wrap:not(body):not(html)
##.layerAdContainer:not(body):not(html)
##.leeads-advert:not(body):not(html)
##.loop-mobile-leeads:not(body):not(html)
##.mittenannons:not(body):not(html)
##.node-sponsored-article:not(body):not(html)
##.nyhet_wrapper_annons:not(body):not(html)
##.o-grid__ad-column:not(body):not(html)
##.penci-adsense-below-slider:not(body):not(html)
##.penci-infeed-fullwidth-ads:not(body):not(html)
##.plista_widget_outstream:not(body):not(html)
##.react-ad:not(body):not(html)
##.rmss_main-ad:not(body):not(html)
##.sponsorBanner:not(body):not(html)
##.sponsrad-artikel:not(body):not(html)
##.swp-ad-strossle:not(body):not(html)
##.sw-popular__article--ad:not(body):not(html)
##.sw-sponsored_post:not(body):not(html)
##.sw-tag-sponsored_post:not(body):not(html)
##.tag-sponsrat-inlagg:not(body):not(html)
##.teaser--native-ad:not(body):not(html)
##.thb_ad_header:not(body):not(html)
##.toppannonser:not(body):not(html)
##.widget_adonnews:not(body):not(html)
##.widget_ev_ad_widget:not(body):not(html)
##.widget_ic_ad_widget:not(body):not(html)
##._ning_outer._ning_jss_zone:not(body):not(html)
##[class*="advads_ad_widget"]:not(body):not(html)
##[id^="adace_ads"]
&autoplay$frame,removeparam=autoplay,domain=di.se|expressen.se
*$ping,domain=fiskejournalen.se
-popup-analytics
-tracking.js$domain=aftonbladet.se|godare.se|livsstil.se|svd.se
/468adrotate.php
/Advertisement$image,domain=sportbloggare.com
/Ad/*$domain=hallbyhandboll.se|skiljebosk.nu
/AffiliateHelper$domain=allas.se|elle.se|femina.se|hant.se|mabra.com|residencemagazine.se|svenskdam.se|motherhood.se
/AiMatch$script,domain=morningstar.se
/AnnonsClickScript.js
/Annons$domain=internetlankar.se
/AudienceTarget$script,domain=morningstar.se
/Banners/webbannons
/BlogPortal/view/Statistics
/CookieBar$script,domain=morningstar.se
/DO-theme/ads.js
/DynamicGAFunctions$script,domain=morningstar.se
/EAS_tag$script
/EUModalDialog$script,domain=morningstar.se
/GA_EEC$domain=osterbottenstidning.fi|sydin.fi|vasabladet.fi
/Global/Annons/*
/Grejer.js$domain=dagensvimmerby.se|dagensvastervik.se|dagenskalmar.nu|dagenshultsfred.se
/HSSAnalyticsUtils.js
/Jofab_Blog/js/ads.min.js
/LoadSlotLocator.$script
/LogRocket.min.js$third-party,domain=~dsc.gg
/OneSignalSDKWorker$script
/Portalannonser/*$image
/QA.js$domain=qruiser.com
/QXA.$script,domain=qx.se|qruiser.com
/Scripts/ads/*$domain=osterbottenstidning.fi|sydin.fi|vasabladet.fi
/Scripts/burt/*
/Script/Ads.js$domain=dagensvimmerby.se|dagensvastervik.se|dagenskalmar.nu|dagenshultsfred.se
/SitesterSurvey*.$script
/Smile_ElasticsuiteTracker/*$script
/SponsorsList$script,domain=hockeyallsvenskan.se
/TSPD/*$script,domain=corren.se|folkbladet.se|mvt.se|nt.se|vt.se|vimmerbytidning.se|kuriren.nu|nsd.se|norran.se|pt.se|ekuriren.se|strengnastidning.se|kkuriren.se|sn.se|eposten.se|unt.se|helagotland.se|kindaposten.se|gotlandjustnu.se
/TopBanner$subdocument,domain=hitta.se
/TrackPageView$domain=mestmotor.se
/Vizzit/vizzit.$script
/Web%20Analytics/*$script
/ab_appnexus_ads
/ab_stats_params$domain=aftonbladet.se|skonhetsredaktorerna.se
/ab_tracking$domain=aftonbladet.se
/adReloader$domain=morningstar.se
/add-ads.js$domain=fria.nu|stockholmsfria.se
/add-page-view$domain=cykla.se
/adform.js$domain=bohuslaningen.se|stromstadstidning.se|markposten.se|harrydaposten.se|partilletidning.se|sttidningen.se|molndalsposten.se|kungalvsposten.se|kungsbackaposten.se|alingsastidning.se|ttela.se|gp.se|hallandsposten.se|hn.se|mellerudsnyheter.se
/adnami/macro$script
/adnuntius_top_scroll
/adn/adn-setup.$script
/adobe/se/target-main-at.js
/adpage$domain=hotellorestaurang.se|byggfakta.today|citymark.today
/ads.article.js
/adsense.index.js$domain=husvagn.se|husbil.se
/ads-countdown.js$domain=aftonbladet.se|livsstil.se|godare.se
/ads-dm.js
/ads.for.me/jsa?$script
/ads.js$domain=flashback.org|onkologiisverige.se
/ads/adnami-conf.js
/ads/global-conf.js
/ads/load-dm.js
/ads?$domain=cirkulation.se
/adtracker$domain=beernews.se
/advertisement-dfp$script
/ad-render$domain=internetmedicin.se
/ad-takeover
/ad-widget
/ad-$image,domain=schack.se
/ad.aspx?
/ad/getNouw.$script
/ad?platform$domain=viaplayradio.se
/ad_acknowledgment$xmlhttprequest
/ad_in_article$script,domain=affarsvarlden.se
/affiliategallery$domain=allas.se|elle.se|femina.se|hant.se|mabra.com|residencemagazine.se|svenskdam.se|motherhood.se
/aftonbladet/crypt/?lpkey$all
/ajax-hit-reg.php?
/ajax/ads.php$domain=garaget.org
/ajax/docu_stats.jsp
/aller-ads
/amplitude$domain=mytaste.se
/analytics$domain=gbgfotboll.se|stff.se|svenskfotboll.se|di.se|etc.se|vackertvader.se|skogsforum.se|skolporten.se
/analytics-bmb
/analytics/cts.min.js
/analytics/gallup
/angry-golick-$script
/annonsbanners
/annonslinje_
/annonssamarbete$xmlhttprequest
/annons$image,domain=dagensvimmerby.se|dagensvastervik.se|dagenskalmar.nu|dagenshultsfred.se
/annons-banner
/annons.aspx?
/annons/banner
/annons_hor.
/annons_ver.
/antiblock$domain=vmj.se|viseniorer.se|danskaspraket.se|digitalavykort.se
/apester-javascript-sdk.min.js
/api/a/b$domain=borskollen.se
/api/log$domain=bohuslaningen.se|stromstadstidning.se|markposten.se|harrydaposten.se|partilletidning.se|sttidningen.se|molndalsposten.se|kungalvsposten.se|kungsbackaposten.se|alingsastidning.se|ttela.se|gp.se|hallandsposten.se|hn.se|mellerudsnyheter.se
/api/natives?$domain=aktuellhallbarhet.se|byggindustrin.se|dagensmedia.se|dagensmedicin.se|fastighetsnytt.se|resume.se|dagenssamhalle.se|market.se|dagligvarunytt.se|privataaffarer.se
/api/sponsors$domain=aikhockey.se|almtuna.com|bikkarlskoga.se|bjorkloven.com|brynas.se|difhockey.se|frolundahockey.com|farjestadbk.se|hockeyallsvenskan.se|hv71.se|ikoskarshamn.se|kalmarhockey.com|leksandsif.se|lhc.eu|luleahockey.se|malmoredhawks.com|modohockey.se|moraik.se|nybrovikings.com|orebrohockey.se|roglebk.se|shl.se|skellefteaaik.se|sodertaljesk.se|taif.nu|timraik.se|vaxjolakers.se|vikhockey.se|vik.se|ostersundik.com
/api/s/track$xhr,domain=eniro.se
/api/tracker?$image
/appinsights/*/track
/appnexus$script
/app.php/adsview$xmlhttprequest
/article-analytics$domain=bulletin.nu
/artikelannons/*
/artiklar/partner$xhr,domain=mestmotor.se
/arto/api/event$domain=arkitekten.se|natursidan.se|svenskfarmaci.se
/assets/DynamicAds-
/assets/js/ads.js$domain=dagensopinion.se
/assets/partnerstat.php?partner=$xmlhttprequest
/assets/site/modules/GTM_
/assets/site/modules/ctm-
/assets/tracking$domain=hornbach.se
/assets/yb_$domain=vackertvader.se
/ast.$script,domain=blocket.se
/atomic-blocks$script,domain=foretagsverige.se|forskningsverige.se|motorbibeln.se|hallbarhetsverige.se|tillvaxtsverige.se|grillbibeln.se|kampenmotcancer.se|folkhalsasverige.se
/atoms/images/*banner$domain=etc.se
/at_banners$domain=alandstidningen.ax
/a?callback=pfmod.saveadsettings
/bannersidor/*
/banners$domain=magasinetparagraf.se|sporttv.nu|cykla.se|vatternrundan.se|dagenstv.com|sydkusten.es|pellesoft.se|dykarna.nu|varmepumpsforum.com|poolforum.se
/banners/annons
/banners/scripts/adx.js
/banners/*casino$image
/banner$domain=revisionsvarlden.se
/banner$domain=thepattayanews.se
/banner/ads/*
/banner?cg$xhr,domain=blocket.se
/betald-exponering$image
/bigdatapushworker.js$domain=eurocampings.se
/bilder-for-annonser$image
/bilder/ads/*
/bilder/annonser/*
/bilder/annons$domain=webbkameror.se
/bilder/betalannonser
/bilder/logotyper/partners
/bilder/sponsorer
/bitcsys/js/bit.js
/block/samarbetspartners$image
/bloggerfy/tracker
/blogpoststatistic/impression
/blogpoststatistic/view
/blogs/log_pageview
/bmbBurt.$script
/bmbDfpUtils.$script
/bmbFusionUtils.$script
/bmb-related-teasers$xmlhttprequest
/bmb/*/native/boosted$xmlhttprequest
/bnrimg$domain=nordiskskog.se
/bnrscr?$domain=motormagasinet.se|food-supply.se|dagenshandel.se|plastnet.se|habit.se|woodnet.se|foodnet.se|transportnet.se|processnet.se|packnet.se|verkstaderna.se|medtechmagazine.se|recyclingnet.se|rt-forum.se|uochd.se|lifesciencesweden.se|fri-kopenskap.se|cleannet.se|framtidensbygg.se|entreprenad.com|metal-supply.se
/brand-metrics$domain=hemnet.se
/bundles/comscore$domain=expressen.se
/bundles/exp-analytics$domain=expressen.se
/bundles/ga-$script,domain=expressen.se
/bundles/parsely$domain=expressen.se
/bunsen/events$domain=yelp.se
/burst-statistics
/casinokollen$all,domain=aftonbladet.se
/casino_utan_licens$image
/cdigo-audit.js
/cecado/advisible.js
/census.js?bust=release
/clickperformance$domain=radio.se
/clicktracking.siteseeker
/closest-native$domain=expressen.se
/cmpv2$domain=m3.se|pcforalla.se|macworld.se
/cmp.js$domain=praktisktbatagande.se|hemtrevligt.se|vagabond.se|tidningenhalsa.se|utemagasinet.se|svenskgolf.se|mestmotor.se|sportfack.se|husohem.se|minhast.se|kalleanka.se|halge.se|bamse.se|akaskidor.se|husvagnochcamping.se|classicmotor.se|scandinavianretro.com
/cm-ad-changer-server
/collect?v$domain=thelocal.se
/content_images/*casino$image,domain=ng.se
/conversions/tracking.js$third-party
/cookieconsent$script,domain=akademiskahus.se|lundagard.se|fuska.nu|kiacarclub.se|nyheteridag.se|internetstart.se|svampguiden.com|scanaktier.se|obosdamallsvenskan.se|elitettan.se|bike.se|runnersworld.se|offside.org
/cookiesCon.js$domain=sydnarkenytt.se
/cookiespolicynotificationbar$domain=svenskahousegruppen.se
/cookies-and-content-security-policy$script,domain=cannabisifokus.se|futsalmagasinet.se|sd.se
/cookie-banner$script,domain=sprintchallenge.se|halsafitness.se
/cookie-consent$script,domain=minhembio.com
/cookie.min.js$domain=assistanskoll.se
/cookie_consent.js$domain=djungeltrumman.se
/cookie_policy.js$domain=nasdaqomxnordic.com
/cookie_popup$script,domain=trafikradion.com|trafik24.se
/cpg_ads.$script
/cs1pc.js$domain=kiaindex.se
/ctr-prd.cbs-measurements.
/cts.js$domain=allas.se|elle.se|femina.se|hant.se|mabra.com|residencemagazine.se|svenskdam.se|motherhood.se
/cx-emediate-userprofile-se
/data/banner$domain=nyaboendet.se
/data/track$domain=nyaboendet.se
/detroitchicago$domain=temadagar.se|svenskaorduttryck.se
/detroitchicago/cmbdv2.js$domain=wernamaten.se
/detroitchicago/denver.js$domain=wernamaten.se
/detroitchicago/*.gif?$image
/dh-adscale$domain=dh.se
/dh-adsticky$domain=dh.se
/dh-voldemort$domain=dh.se
/dialog$script,domain=marknadschefer.se
/discourse-adplugin
/discourse-prisjakt
/discourse-revive
/docunet_stats.js
/dovas/ads/*
/downloads.mailchimp.com/js/signup-forms/popup
/dyTracker.js?bust=release
/dynamic-yield/report/pageview
/egmont-ads
/egmont-continuous-scroll/continuous-scroll-analytics.js
/egmont-streamlined-ads
/elasticsuite/tracker
/emediate-responsive-wp-plugin
/empty.html$subdocument,domain=hotellorestaurang.se|byggfakta.today|omtanke.today|citymark.today
/enklare-banners/enklare-torgetgruppen
/entag.$script,domain=leta.se
/entryclick;_
/ess.eurovator.se/*
/eu_cookie_compliance$script,domain=industrinyheter.se|dagensnaringsliv.se|infrastrukturnyheter.se|sportochfritidsnyheter.se|inredningsnyheter.se|byggnyheter.se|dagensfastigheter.se|stockholmsbyggnyheter.se|energinyheter.se|vindkraftsnyheter.se|solenerginyheter.se|jarnvagsnyheter.se|transportochlogistik.se|metallerochgruvor.se|papperochmassa.se|miningmetalnews.com|visitskane.com|ergo.nu|ki.se|sxk.se
/evidon*.js$domain=morningstar.se
/exposure$xmlhttprequest,domain=lokalguiden.se
/expressen/crypt/?lpkey$all
/ext/phpbb/ads/*
/ezoic$domain=temadagar.se
/facebook_tracking_pixel$script
/fb_pixel.js
/featured/promotion$domain=borskollen.se
/filarkiv/bilderbanner/*
/firebase-analytics.js$domain=stoppapressarna.se
/flex-mag/js/dfp.js
/footer/ad|
/foretagarna.usercentrics.js$domain=foretagarna.se
/forumannons.$subdocument,image,script
/forum/assets/google-tag-manager
/forum/images/_banners
/forum/img/banners
/fptools.js$domain=allas.se|elle.se|femina.se|hant.se|mabra.com|residencemagazine.se|svenskdam.se|motherhood.se
/frontendLogger$domain=flashscore.se
/fullpageAd.js
/fullpage$script,domain=poddtoppen.se
/fullpage-ad.js
/fusionadloader.$script
/ga.js$domain=helgon.se
/ga_cookie_track.js
/gdprlock$third-party
/gdpr/*$domain=visitlulea.se|husbilskompisar.se|rotter.se|luleabusinessregion.se
/getAdById.php?
/getadd$domain=bovision.se
/get.aspx?AdSlotID$script
/glimr$script,domain=aftonbladet.se|blocket.se|livsstil.se|godare.se
/glimr-static$domain=~klart.se
/googleanalytics.js$domain=fria.nu|stockholmsfria.se
/google-analytics$domain=teknikveckan.se
/google-analytics-for-wordpress$important,script,xmlhttprequest
/google-analytics-premium$important,script
/google-gpt.js$domain=alekuriren.se
/google-tag-manager$domain=hemnet.se
/google-universal-analytics$script
/gpAnalytics$script
/gplus.php$script,domain=fria.nu|stockholmsfria.se
/gtagEventTracker.js
/gtm-sokande.js$domain=antagning.se|universityadmissions.se
/gtm-*.appspot.com
/headerbidding.js
/healthcare-puffar$domain=dh.se
/helios/multiad_jquery
/hemmafixbloggen/includes/events-tracker
/home/ads$domain=allastudier.se
/hotjar/hotjar.script.js
/hrnytt/banner$domain=hrnytt.se
/html5videovastplugin.js$domain=skidspar.se
/iab/iab.js
/idle.min.js$domain=180.se
/iframeadvloader.$script
/illustrationer/annons_
/images/site/annonser
/images/*casino$domain=festivalinfo.se
/img/allalanse$image,domain=ekonominyheter.se
/img/banklan/*$image,domain=ekonominyheter.se
/img/bettingstugan.$image
/img/compricer$image,domain=ekonominyheter.se
/impression$script,domain=affarsvarlden.se
/integrations/adwords$important,domain=dagen.se
/integrations/facebook-pixel$important,domain=dagen.se
/integrations/google-$important,domain=dagen.se
/isbanner/ib.js
/javascript_nbenhadverts/*
/jquery.smartbanner.js$domain=kristendate.se
/js/OneSignal.js
/js/PerimeterX$domain=skyscanner.se
/js/adLocker.
/js/annons.js
/js/byside_webcare
/js/external.php$domain=hockeysnack.com
/js/fullpageads.js
/js/iepngfix_tilebg
/js/improve_digital_ads
/js/infinite-ads
/js/intelecom.tracker
/js/sifo.js
/js/sticky-mobile-ad
/js/userneeds.
/jwpsrv.js$domain=aftonbladet.se|svd.se|tv.nu|axess.se|freeride.se|happyride.se|embed.futuresportsmedia.com|streamio.com|laget.se|moviezine.se|fasttrack.webstream.dk|cdn.jwplayer.com|livsstil.se|allas.se|elle.se|femina.se|hant.se|mabra.com|residencemagazine.se|svenskdam.se|motherhood.se|godare.se|recept.se|hastnet.se|skippo.se
/keremiya1/js/addtoany.js$script,important
/lasso-performance
/lazyad-loader.$script
/lazyload-ad.$script
/leeads-fullpage.js
/leeads_takeover$script
/linguee/statistics
/linkpulse/*$script
/links/*casino*.$domain=emocore.se
/live/radarmagazine.se.js
/loada.forum.$script
/load_ads.js$domain=koket.se
/logger/logger?
/logotyper/sponsorer-partners
/logs/client$domain=swebbtv.se
/log/hublytics
/log|$domain=booli.se
/log|$domain=vk.se|folkbladet.nu|nordsverige.se|mellanbygden.nu|vasterbottningen.se|lokaltidningen.nu
/losad/loada.$script
/maps.sponsored-pill.$script,domain=tripadvisor.se
/marbles/marbles.js
/marknadsguiden.$frame,domain=barometern.se|blt.se|bt.se|kristianstadsbladet.se|olandsbladet.se|smp.se|sydostran.se|trelleborgsallehanda.se|ut.se|ystadsallehanda.se|vxonews.se|vaxjobladet.se|nsk.se|klt.nu
/maxetise$domain=teknikveckan.se
/mb-admanager.js?
/media/eventad/*
/media/partners$domain=hockeynews.se|tvmatchen.nu
/mediehuset-gront/img/*annons
/mediehuset-gront/img/*banner
/meetrics-tracker
/mega.$domain=vk.se|folkbladet.nu|nordsverige.se|mellanbygden.nu|vasterbottningen.se|lokaltidningen.nu
/metrics$domain=swebbtv.se
/metrics/bambuser
/minbostadstatic/js/partner/*
/modal.js$script,domain=alltforforaldrar.se
/mod_carousel_banner$domain=bjuvsweek.se
/monetization/ads-module/*
/monetization/pixel-sdk/*
/mp_emediate/inc/annons.html
/mrbet_banner
/native$domain=sydnarkenytt.se
/native-ads$domain=atl.nu|landlantbruk.se|land.se
/native-article-campaigns$domain=allas.se|elle.se|femina.se|hant.se|mabra.com|residencemagazine.se|svenskdam.se|motherhood.se
/native.html$domain=allas.se|elle.se|femina.se|hant.se|mabra.com|residencemagazine.se|svenskdam.se|motherhood.se
/newsner-ad$domain=newsner.com|humorbibeln.se|sportbibeln.se|ettgottskratt.se|djurbibeln.se
/newsner-stats$domain=newsner.com|humorbibeln.se|sportbibeln.se|ettgottskratt.se|djurbibeln.se
/noview.$script,domain=trafikradion.com|gofm.se|trafik24.se
/nyhetsspalt_banner_js
/omniture/s_code.js
/one-signal$domain=swebbtv.se
/opus-analytics
/ordmedzcxy_files/ads$domain=ordmedzcxy.se
/pageView$xhr,domain=altinget.se
/pagead$domain=vilaser.se|horoskoptid.se|eniro.se
/pages/native$domain=aktuellhallbarhet.se|byggindustrin.se|dagensmedia.se|dagensmedicin.se|fastighetsnytt.se|resume.se|dagenssamhalle.se|market.se|dagligvarunytt.se|privataaffarer.se
/pages/tag$domain=aktuellhallbarhet.se|byggindustrin.se|dagensmedia.se|dagensmedicin.se|fastighetsnytt.se|resume.se|dagenssamhalle.se|market.se|dagligvarunytt.se|privataaffarer.se
/peertube-plugin-google-analytics
/permutive-async.js
/pfizer_analytics
/phaser-ads.min.js$script
/pixel/impression$domain=skyscanner.se
/playbuzz-ads-core
/player-plugin-ad$domain=tv.aftonbladet.se
/player-plugin-sponsor$domain=tv.aftonbladet.se
/player-plugin-tracking$domain=tv.aftonbladet.se
/plugins-mu/analytics
/plugins/add-to-any$script
/plugins/adlounge
/plugins/adsanity
/plugins/adsense%20click%20proctect
/plugins/ad-ace
/plugins/ad-blocking-advisor
/plugins/affiliate$script,domain=56kilo.se
/plugins/afp-default-pricetable/js/ga-tracking
/plugins/all-in-one-seo-pack$script
/plugins/analytics-insights
/plugins/angwp
/plugins/annonstorget$script
/plugins/appbanners/*
/plugins/ap-plugin-scripteo
/plugins/arscode-social-slider
/plugins/beautiful-and-responsive-cookie-consent$script,domain=melodifestivalklubben.se
/plugins/better-adsmanager/*$~stylesheet
/plugins/bfp-popup$script,domain=omtanke.today
/plugins/blog-analytics
/plugins/bmb-dfp-plugin
/plugins/borlabs-cookie$script,domain=alltombrollop.com
/plugins/boxzilla$script,domain=dialasen.com|arbetaren.se
/plugins/bravepopup$script,domain=matkasse.se|tidningenglobal.se|fempers.se
/plugins/bsa-plugin-pro-scripteo
/plugins/cardoza-facebook-like-box
/plugins/chimpy/*
/plugins/christmas-panda
/plugins/cm-pop-up-banners
/plugins/cm-takeover-ad
/plugins/complianz-gdpr$domain=iconmagazine.se|signprint.se|vilaser.se|arjeplognytt.se|aftonkuriren.se|tidningenglobal.se|tidningensyre.se|landetsfria.nu|fempers.se|macken.xyz|webb-tv.nu|kalmar.nu|brollopsmagasinet.se|megafonen.se|radiotreby.se|revisionsvarlden.se|kyrka.se|nuiroslagen.se|tlnt.se|sjofartstidningen.se|pensionarsliv.se
/plugins/consent-magic-pro$script,domain=namnmarkning.se|bluum.se|gobokhandeln.se
/plugins/content-hub-wp-plugin/assets/js/hub-time-spent
/plugins/convertplug
/plugins/convertpro
/plugins/cookie-law-info$script,domain=gilla.se|startaochdriva.se|sverige.nu|conpot.se|firstclassmagazine.se|magasinetkonkret.se|kvalitetsmagasinet.se|miljo-utveckling.se|telekomidag.se|vdtidningen.se|gullislastips.se|nyfiknainvesterare.se|discoveringtheplanet.com|bussmagasinet.se|torbjornstips.se|affarsstaden.se|marknadschefer.se|automation.se|dinbyggare.se|aktieskolan.se|insikt24.se|skogen.se
/plugins/cookie-notice$script,domain=bildobubbla.se|zeromagazine.nu|sverigespringer.se|gasetten.se|sillyseason.se|gentlemannaguiden.com|matmalin.se|svensktidskrift.se|schack.se|densistavilan.se|horisontmagasin.se|kobe.se|tidningenproffs.se|jaktojagare.se|tobaksfakta.se|bebisvarlden.se|underbaraclaras.se|cykelframjandet.se|dalabygden.se|lansposten.se|sormlandsbygden.se|vaguiden.se|grandtech.se
/plugins/cookie-popup$script,domain=skillingaryd.nu|xn--vrnamo-bua.nu
/plugins/cresta-social-share-counter
/plugins/custom-banners$domain=skolfamiljen.se
/plugins/daftplug-instantify$domain=se.moyens.net
/plugins/deblocker/js/deblocker$script,domain=~filecr.com
/plugins/dohi-sellbranch/js/popup$script
/plugins/doubleclick-wp
/plugins/dsgvo-tools-cookie$script,domain=motorsport4sale.com
/plugins/duracelltomi-google-tag-manager
/plugins/easy-adsense
/plugins/easy-affiliate-links
/plugins/easy-facebook-likebox$script
/plugins/easy-social-sharing$script
/plugins/elfsight-social-share-buttons
/plugins/embedpress/assets/js/ads.js
/plugins/exit-popup/*$script
/plugins/facebook-conversion-pixel
/plugins/facebook-ogg-meta-tags
/plugins/facebook-pagelike-widget
/plugins/facebook-popout-likebox
/plugins/fisher/core/js/generated/analytics.js
/plugins/fisher/core/js/generated/fixed-panorama
/plugins/fisher/core/js/generated/infinite-ads
/plugins/ga-germanized/*
/plugins/ga-in/*
/plugins/gdpr-cookie-compliance$domain=goteborgsgolfaren.se|nyhetersto.se|modernalivet.se
/plugins/genesis-simple-share$script
/plugins/ginger/addon/analytics/*
/plugins/google-analytics
/plugins/google-analytics-dashboard$important,script
/plugins/hemmafix-facebooklike
/plugins/host-analyticsjs-local
/plugins/hustle/*$script
/plugins/icegram
/plugins/iis-mailchimp
/plugins/interscroller-ads
/plugins/interstitial-ads
/plugins/jet-popup$domain=javligtgott.se
/plugins/jnews-social-share/*$script
/plugins/koko-analytics
/plugins/lbg-audio8-html5-radio_ads
/plugins/leeads-
/plugins/likebtn-like-button/*
/plugins/madonltd-full-screen-ad
/plugins/mailpoet/*$script,domain=~sameforeningen-stockholm.se
/plugins/mashshare
/plugins/material-admin/visitor-stats$script
/plugins/mediaconnect$domain=fof.se|spraktidningen.se|elinstallatoren.se|modernpsykologi.se|vvsforum.se
/plugins/metro-affiliate
/plugins/mitti-adform
/plugins/ml-adverts
/plugins/monsterinsights$script
/plugins/newsletter$script,domain=56kilo.se
/plugins/newsletter-leads/libs/simplemodal$script
/plugins/newsner-lead-tracking
/plugins/notificationx$script
/plugins/no-right-click-images-plugin$script
/plugins/ns-facebook-pixel
/plugins/official-facebook-pixel
/plugins/onesignal-free-web-push-notifications
/plugins/optin-cat-elite-wp$script
/plugins/page-views-count
/plugins/pc-google-analytics
/plugins/pixelyoursite
/plugins/pixel-caffeine
/plugins/pixel-cat
/plugins/popups/*$script,domain=svenskhistoria.se|bugburger.se
/plugins/popup$domain=ordfrontmagasin.se|snowmobile.se|forvaltarforum.se|it-finans.se|it-halsa.se|it-kanalen.se|it-pedagogen.se|it-retail.se|jobsinsweden.se
/plugins/pum-$script,domain=snowmobile.se|it-finans.se|it-halsa.se|it-kanalen.se|it-pedagogen.se|it-retail.se
/plugins/quantcast-choice$script,domain=handbollskanalen.se|javligtgott.se|dh.se
/plugins/quick-adsense
/plugins/r9-analytics
/plugins/random-banner
/plugins/sandviks-weblog$script,domain=bebisvarlden.se
/plugins/sassy-social-share/*$script,domain=~nova.rs
/plugins/sea-short-stats
/plugins/seo-automated-link-building
/plugins/se-wordpress-affiliatehelper
/plugins/share-and-follow/*
/plugins/simple-banner
/plugins/simple-social-buttons$script
/plugins/skydda-advisor
/plugins/socialsnap$script
/plugins/social-pug
/plugins/social-warfare$script,domain=varvat.se
/plugins/srs-simple-hits-counter
/plugins/statebuilt-facebook-page-like-popup
/plugins/sticky-facebook-banner$script
/plugins/super-socializer$script,domain=sportbilen.se
/plugins/svenskaspel-$script
/plugins/sw-ad-inserter
/plugins/sw_ad_inserter
/plugins/the-moneytizer/*$script
/plugins/thrive-leads
/plugins/trackable-social-share-icons
/plugins/triggerbee/*
/plugins/uk-cookie-consent$script,domain=cykla.se
/plugins/ultimate-social-deux$script,domain=totallyorebro.se|totallystockholm.se
/plugins/ultimate-social-media-$image,script
/plugins/ungrabber
/plugins/vizzit-analytics
/plugins/wccp-pro$domain=dinbyggare.se
/plugins/webtoffee-gdpr-cookie-consent$domain=forskning.se|hejaolika.se|kvartal.se|karriarlakare.se|svenskfilmdatabas.se|bredband.se
/plugins/wf-cookie-consent$script,domain=spelochfilm.se
/plugins/woocommerce-google-adwords
/plugins/wordpress-stats-manager-pro
/plugins/wplinktrade
/plugins/wpx-bannerize$script
/plugins/wp-adsense
/plugins/wp-analytify
/plugins/wp-auto-affiliate
/plugins/wp-banner-manager
/plugins/wp-click-info
/plugins/wp-content-copy-protection
/plugins/wp-copy-protect
/plugins/wp-evolve-gpt
/plugins/wp-facebook-pixel
/plugins/wp-gdpr-compliance$script,domain=pussad.se
/plugins/wp-lrf-paywall
/plugins/wp-popups-lite$domain=grillbaronen.se|spelochfilm.se|sameforeningen-stockholm.se|norrkopingshistoria.se
/plugins/wp-power-stats
/plugins/wp-snow-effect
/plugins/wp-statistics
/plugins/wp-stats-manager
/plugins/wysija-newsletters
/plugins/yeloni-free-exit-popup
/plugins/yuzo/public/assets/js/pixel-geo
/pogoadkit.js$domain=nordic.ign.com
/popup-subscribe.js$domain=borsvarlden.com
/popup/follow-us-fb
/prebid_rtb_call
/prisjakt$xmlhttprequest,domain=fz.se
/private-browsing.js$domain=thelocal.se
/prod/adform
/profile$ping,domain=feber.se|skippo.se|tasteline.com|tjock.se|veckorevyn.com|marcusoscarsson.se|handbollskanalen.se|surfa.se|nordichardware.se|hockeynews.se|tv4.se|fotbollskanalen.se|koket.se|teknikveckan.se|56kilo.se
/promoted_ads$domain=bostadsportal.se
/ps-partner$xmlhttprequest,domain=dagensps.se
/publicPartners$domain=familjehemsbanken.se|familjehemmet.se
/public/log$domain=kalender.se
/pulsetracking$script
/pum/*$domain=flm.nu|dagenslogistik.se|battrestadsdel.se|skaneplus.se
/qc_cmp$domain=reseguiden.se
/questback.popup$script
/rantekartan$subdocument,domain=expressen.se
/raven$script,domain=mitti.se|travnet.se|nyheter24.se|tyda.se
/recommendations$xmlhttprequest,domain=expressen.se
/registerhit?$image
/renderBanner.do?zoneId=
/resource.ifragasatt.se/sd-ads
/retargeting-pixels
/revive.js$domain=skidspar.se
/revive/revivejs.php$script
/revive/www/images$image
/rubiconproject_prebid
/scripts/js3caf.js
/scripts/leeads-
/scripts/opt/view.analytics.js
/script.js$3p,domain=spelkritik.se
/seenthis-hub$script
/se-ads-microservice
/se-calico/bundle.js
/se-ocelot/bundle.js
/se-recommendation-microservice$domain=allas.se|elle.se|femina.se|hant.se|mabra.com|residencemagazine.se|svenskdam.se|motherhood.se
/sg_reklam$domain=svampguiden.com
/sh404sefsocial$script
/sharedaddy/sharing.$script
/shared/crm-campaign-handler.js$script
/sharethis.js$domain=allsvenskan.se|superettan.se
/sidebar-ads
/siforesponsivemeasure
/sifo-tracking.js
/sifo_analytics
/sifo_msr
/site_media/annons
/skolvarlden_theme/js/s_code.js
/skrattnetdotse/js-ck.js
/skrattnetdotse/js-xdp.js
/smartBanner.js$domain=hant.se|svenskdam.se
/snowday262.js
/snowfall.jquery.min.js
/snowfall.min.jquery.js
/snowplow$script,domain=~rossmann.pl|~prolific.co|~nrk.no
/soledad/js/detector.js
/sounds/chimes.mp3$domain=skaneplus.se
/spec/adsm.macro.
/sponsoredLink.js$domain=fotbolltransfers.com
/sponsored_articles$domain=fastighetssverige.se
/sponsorloggor$domain=swehockey.se
/sponsors$domain=sdhl.se|storvretaibk.se|obosdamallsvenskan.se|elitettan.se
/spotlight-ad_$image
/ss_foundation/combined_li_tracking
/static.marklar.se/*-tracker
/static/js/loada.js
/static/media/*casino$domain=dagenstv.com|kolla.tv
/statistics/statistics.js
/statistics/statistics.php
/stats.wp.com$script
/stats/ewstats.
/stats/stats.asp?
/sticky-ads$script
/strossle-analytics.js
/strossle-start-page-ad$xmlhttprequest
/strossle-widget
/sunt/mainfeed
/sunt/sidefeed
/sveacasino_banner
/svenska-ridsportforbundet/*banners
/svff/bannerblock/*
/sv_se/metrics/*$script,xmlhttprequest
/swordfishinc.download.akamai.com/*$script
/synonymerse-adapter.js$domain=synonymer.se
/tabs_hits_counter.php$image
/takeover-ad.js$domain=ridsport.se
/takeover.js$domain=gekas.se
/tasteline/templates/popup
/tbilen/banner/*
/templates/ad_$domain=jaktojagare.se
/thumbnail_bettingstugan$image
/thumbs/webbannons$image
/tinypass-gtp.min.js
/toppbanner.js$domain=sydnarkenytt.se
/toppbanner_snippet_js
/torgen/banner.stat
/trace$xhr,domain=netflixguiden.se|radio.se
/trackers/SessionCam-tag
/tracker.php?do$image
/tracker/socket$domain=swebbtv.se
/tracking.php?aid=
/tracking/cts.js
/tracking/fpc.js
/track.js$domain=destination.se|sistaminuten.se
/track/view?webInteractiveId$image
/trafikfonden/*
/tvg-legacy-splash-redirector/public/t/*
/tvg-redirector/public/t/*
/tv/annons$domain=expressen.se
/tv/brand-studio$domain=expressen.se
/tv/sponsrat$domain=expressen.se
/twitter_count.php$domain=fria.nu|stockholmsfria.se
/ub-ads/*$script
/unica/html-banners
/uploads/annonser
/uploads/bilder/Banner/*
/uploads/bilder/Samarbetspartners
/upload/puff/*$domain=bergsmannen.se|tidningenbyggmaterial.se|tidningendacksnack.se
/usabilla$script
/users/2401/*$image,domain=ng.se
/user_behaviour_data$domain=skyscanner.se
/utag$script,domain=gaffa.se
/utag/aller-media
/vestigo$domain=momondo.se
/vgc/cdn/js/libs/ast/*$script,domain=aftonbladet.se
/videojs-preroll$domain=himlentv7.se
/videojs.ima.$domain=sportbladetplay.se|staylive.tv
/viewed$xmlhttprequest,domain=fotbolltransfers.com
/view_count/view.php
/view_count/view$domain=byggahus.se
/visit/v.js
/wdg/iab-active
/wds_nyhetsbrev_popup
/webbresurser/banner/*
/white_pixel.gif$domain=byggfakta.today
/wordads-classes/js/*
/workbox-offline-ga$domain=magasinetkonkret.se
/wpbm-banners/*$image
/wp-content/banners$image
/wp-content/plugins/addthis/*
/wp-content/plugins/easy-social-share-buttons$script
/wp-content/plugins/email-subscribe$script
/wp-content/plugins/top-10/*$script
/wp-content/static/unruly.js$script
/wp-content/themes/keremiya1/js/jopper.
/wp-content/themes/keremiya1/js/license.
/wp-content/themes/keremiya1/js/script.js
/wp-content/uploads/html5ads/*
/wp-content/uploads/*Casinodealen$image
/wp-content/uploads/*LeoVegas$image
/wp-content/uploads/*annons$image,domain=~datahjelperne.no|~dataliner.no|~annonsere.gulesider.no
/wp-content/uploads/*banner$image,domain=marsta.nu|alltomhif.se|branschkoll.se|brollopsmagasinet.se|bussmagasinet.se|danstidningen.se|guldkanalen.se|katerinamagasin.se|ljuskultur.se|sportpanelen.se|turismnytt.se|opulens.se|borattforum.se|dental24.se|tekniknytt.se|pakryss.se|investerarbrevet.se|svensktidskrift.se|electronic.se|restaurangvarlden.se|finanstid.se|naringslivetvgl.se|dalarnasaffarer.se|stockholmsaffarer.se|jamtlandsaffarer.se|hallandsnaringsliv.se|sjuharadsnaringsliv.se|battregolf.se|svenskhistoria.se|arjeplognytt.se|bioenergitidningen.se|fisheco.se|autonytt.se|zeromagazine.nu|improveme.se|dagensinfrastruktur.se|nordiskaprojekt.se|svenskbyggtidning.se|grontsamhallsbyggande.se|alekuriren.se|realtid.se|golfguidenonline.se
/wp-content/uploads/*betfair$image
/wp-content/uploads/*bethard$image
/wp-content/uploads/*bettingkollen$image
/wp-content/uploads/*bettingstugan$image
/wp-content/uploads/*betting$image,domain=nyadagbladet.se|kulturbloggen.com|hockeybladet.nu|newsvoice.se|spelochfilm.se|bandyfeber.com|battrestadsdel.se
/wp-content/uploads/*casinoutan$image
/wp-content/uploads/*casino$image,domain=nyadagbladet.se|kulturbloggen.com|newsvoice.se|svenskhistoria.se|battrestadsdel.se|zeromagazine.nu|totallyorebro.se|totallystockholm.se|djungeltrumman.se|vaken.se|tekniknytt.se|kingsizemag.se|spelochfilm.se|macken.xyz|improveme.se|bandyfeber.com|stoppapressarna.se|dagensinfrastruktur.se|nyaprojekt.se|nordiskaprojekt.se|svenskbyggtidning.se|grontsamhallsbyggande.se|sjostadsbladet.se|autonytt.se|hockeybladet.nu|tv-kanal.se
/wp-content/uploads/*kasino$image,domain=improveme.se|sjostadsbladet.se
/wp-content/uploads/*mrgreen$image
/wp-content/uploads/*ninjacasino$image
/wp-content/uploads/*noaccountbet$image
/wp-content/uploads/*oddsbonusar$image
/wp-content/uploads/*reklam$image,domain=hockeyettan.se
/wp-content/uploads/*svea-casino$image
/wp-content/uploads/*svenskacasinoonline$image
/wp-content/uploads/*unibet$image
/wp-content/uploads/*-sidebar$image,domain=dagensinfrastruktur.se|nyaprojekt.se|nordiskaprojekt.se|svenskbyggtidning.se|grontsamhallsbyggande.se
/wp-content/uploads/*/public/assets/js/advanced.js$script
/wp-content\/uploads\/[0-9]+/$script,domain=skanesport.se|dackavisen.se|automation.se|tidningenproffs.se|densistavilan.se|universitetslararen.se|alekuriren.se
/wp-json/wpstatistics
/wp-json/wp-statistics
/wp-native-ads.json
/ws-tracking$domain=voister.se
/ws-tracking.js$domain=tidningenbalans.se
/www.livsstil.se\/cnp-assets\/[0-9]+./$script,domain=livsstil.se
/www/images/*$domain=elektronikforumet.com
/xhr-ads.min.js
/xhr/b/s$domain=skyscanner.se
/zad.js$domain=nordic.ign.com
/zdadkit$domain=nordic.ign.com
/*banner-nyhetsbrev*.mp4
/?adsforwp_front_js
/?agg_url=/shopping$domain=nyheter24.se
/?agg_url=/sponsratinnehall$domain=nyheter24.se
/?client=ca-pub-$script
/?dtbnrspcid=$xmlhttprequest
/?file=lokus$subdocument
/?news=ajaxrequest&ArtSponsor
/?news=ajaxrequest&bannerlinks
/?news=ajaxrequest&bannerzone
/?news=ajaxrequest&blok=sliderBanner
/?template=prisjakt$domain=ljudochbild.se
/?trafikkalla$image,domain=bloggplatsen.se
/_adsmodern/*$image
/_api/*/visit$domain=placera.se
/_graphics/annons
/_papers_media/banners
/_sites_media/*/uploads/Banners
/_t/se.js$domain=hornbach.se
/_vercel/insights/*
://gtm.*.js?id=GTM
://gtm.*/g/collect?
://impression-tracker-service
://sifomedia.
?action=advanced-ads-tracking-track
?action=get_banners$domain=djungeltrumman.se
?autoPlay$frame,removeparam=autoPlay,domain=expressen.se
?autoplay=true$frame,removeparam=autoplay,domain=expressen.se
?url=*impse.tradedoubler.com$image
@@/adserver.$script,~third-party,domain=fotosidan.se|utsidan.se
@@/advert.js$1p,domain=aktuellhallbarhet.se|byggindustrin.se|dagensmedia.se|dagensmedicin.se|fastighetsnytt.se|resume.se|dagenssamhalle.se|market.se|dagligvarunytt.se|privataaffarer.se
@@/adx.js$~third-party,domain=atl.nu|landlantbruk.se|land.se
@@/ad-block-detection-script$domain=blocket.se
@@/aff/images/*$image,domain=alltforforaldrar.se
@@/appbanner.jpg$image,domain=guldkanalen.se
@@/assets/ads-dm.js$~third-party,domain=corren.se|folkbladet.se|mvt.se|nt.se|vt.se|vimmerbytidning.se|kuriren.nu|nsd.se|norran.se|pt.se|ekuriren.se|strengnastidning.se|kkuriren.se|sn.se|eposten.se|unt.se|helagotland.se|kindaposten.se|gotlandjustnu.se
@@/freemium/di/analytics$script,domain=di.se
@@/lazy_load.js?gcb$domain=hemmanytt.se
@@/plugins/ad-ace/*/adblock-detector
@@/plugins/convertplug/modules/modal/*/cross.png$image,~third-party
@@/scripts/advert_$~third-party,domain=di.se
@@_advert.$domain=e-pages.dk
@@||cargodisplayads.com/gota/api/v1/adImage$image,domain=barometern.se|blt.se|bt.se|kristianstadsbladet.se|olandsbladet.se|smp.se|sydostran.se|trelleborgsallehanda.se|ut.se|ystadsallehanda.se|vxonews.se|vaxjobladet.se|nsk.se|klt.nu
@@||cargodisplayads.com/till_minne/
@@||cdn.play.showheroes.com/part/partimage$image
@@||cdn.play.showheroes.com/part/rendered$media
@@||createsend1.com/css/
@@||feed.meltwater.com^$subdocument
@@||fwmrm.net/ad/g/$xhr,domain=tv4play.se|tv4.se|fotbollskanalen.se|koket.se
@@||fwmrm.net/crossdomain.xml$domain=embed.viaplay.com
@@||img.upsales.com^
@@||js.createsend1.com/js/jquery
@@||js.driftt.com^$domain=sanity.io
@@||klaviyo.com/media/js/public/klaviyo_subscribe.js$domain=solostove.com
@@||kritiker.se^$generichide
@@||marketo.com^*/form
@@||monetize-static.viralize.tv/viralize_player_content$script,xhr
@@||nuthymia-llc.ck.page/*/index.js$domain=nickwignall.com
@@||pages.upsales.com^
@@||www.googletagmanager.com/gtm.js$script,domain=elgiganten.se
||1terms.com^
||123on.com/images/pixel
||123on.com/logs
||123on.com/static/videojs.pulse
||172.104.145.13^
||ab.fastighetsvarlden.se^$script
||accesslnk.com^
||activate.social^$third-party
||activehosted.com^$third-party
||addrevenue.io^$third-party
||addsleeper.com^$third-party
||addtoany.com^$third-party
||adeprimo.se^$third-party
||adfenix.com^$third-party
||adhype-assets.com/images/*betting
||adhype-assets.com/images/*casino
||adhype.se/js/native
||adnordics.com^$third-party
||adonsales.com^$third-party
||adonstudio.com^$third-party
||adviral.s3.amazonaws.com/sponsored/
||advisa.se^$third-party
||advisible.com^$third-party
||ad.iplayer.org^$third-party
||affiliatable.io^$third-party
||affiliator.com^$third-party
||aff.bstatic.com^$third-party
||aftonbladet.se.*.$document
||agency360.io^$third-party
||ajs-assets.ftstatic.com/ftUtils.js
||akademiskahus.se/AddThis?$script
||alkemi.com.se^
||allaaktier.se/ads/
||allastudier.se/TrackingSearch
||allastudier.se/search-sponsor
||allsvenskan.se/allsvenskan-script-min.js
||alphalete.com.se^
||amazonaws.com/adn-tag
||amazonaws.com/adsfallback/
||amazonaws.com/metapic-cdn/*/metapic.
||amazonaws.com/pfe_im/js/prod/pcc/s_code.js
||analytics-smhise.smhi.se^
||analytics.barnebys.sh^$image
||analytics.gen.shield.monitoringservice.co^
||analytics.ozzi.io^$third-party
||analytics.teknikveckan.se^
||analytics.undeco.se^
||apis.google.com/js/plusone.js$third-party
||api-sa.rikatillsammans.se^
||api.hitta.se/creepy
||api.hitta.se/offer
||api.hitta.se/partnerintegration
||api.hitta.se/statistics
||api.mpzmail.com/tracker
||api.netb11.com/b/$image
||api.staylive.tv/videos/engagement
||applets.ebxcdn.com/ebx.js$domain=stoppapressarna.se
||applicationinsights.azure.com/*track
||app.termly.io^$domain=soderkopingsposten.se
||apsis.one^$third-party
||ascontentcloud.com^$third-party
||aservice.tools^
||assets.pinterest.com/js/pinit$third-party
||assets.tumblr.com/share-button.js$third-party
||assets.voyado.com/jsfiles/analytics
||assistanskoll.se/images/banner
||atl.nu/api/mnews
||atmtd.com^$third-party
||auction-release.mlpapi.com/site/LoadPluginSite
||aventyret.com^$third-party
||aweber.com^$third-party
||axess.se^*/track-views
||azurewebsites.net/partnerArticle
||bannerutbyte.se^$third-party
||barbours.com.se^
||barnebys.sh/js/btag
||bcm.interactives.dk/script/
||bellmetric.net^$third-party
||best-prizes-now.$all
||bettingstugan.se^$third-party
||biddercore.io^$third-party
||bilweb.se^$third-party
||biowebb-data.*.amazonaws$important,third-party
||bio.se/js/googleAnalytics.js
||bjuvsweek.se/images/*annons
||blocket.se^$third-party
||bloggportalen.se^*/blogstat.js
||blogg.se/plugin/ads.js
||blogg.se/public/js/metrics
||blogg.se/shared/js/bloggse.js
||bloglovin.com^$third-party
||bokmassan.se/wp-json/*/ad/
||boktugg.se/wp-content/cache/min/1/pa-
||bonniergaming.com^$third-party
||borsvarlden-banners.azurewebsites.net^
||borsvarlden.com/banners/
||borsvarlden.com/js/cookie-notice
||brandy.bonniernewslifestyle.se^
||breakit.se/js/ads/
||breakit.se/js/facebook
||breakit.se/js/google-analytics
||breakit.se/js/hotjar
||bstatic.com/static/affiliate$third-party,~stylesheet
||btcswe.com^$third-party
||buzzador.com^$third-party
||bwz.se^$third-party
||bytbil.com/bundles/js/tracking
||bytelab.dk^$third-party
||cargodisplayads.com^$third-party
||carneoam.com/advert/
||cartbooster.io^$third-party
||casinotoplists.com^$third-party
||casinoutankonto.net^$third-party
||casono.se^$third-party
||ccpa.sp-prod.net^$domain=m3.se|pcforalla.se|macworld.se|computersweden.se
||cdn-cookieyes.com^$domain=lokalti.se|jarnvagar.nu|senses.se|norrmejerier.se|temadagar.se|smartsenior.se|tekniknytt.se|nordigt.se|autonytt.se|vm-fotboll.se|kak.se|smhi.se|borattforum.se|mis.se|universitetslararen.se|em-fotboll.se|lakemedelsvarlden.se|samfalligheterna.se|husbilsplats.se|katerinamagasin.se|dagenslogistik.se|biostock.se|skellefteaworks.se|datormagazin.se|travnet.se|malarbok.nu|barn-filmer.se|matmenyer.se|sunnenytt.se
||cdn-sitegainer.com/sitegainer
||cdn.adt*/atag.js?$third-party
||cdn.adt*/jsTag?$third-party
||cdn.advisible.com/accl
||cdn.advisible.com/adk
||cdn.aller.se/cts/
||cdn.livechatinc.com/tracking$domain=~box.co.uk
||cdn.svenskalag.se/img/sponsors$image
||centotag.io^$third-party
||cervera.se/t/t?
||championsverige.com.se^
||cision.com^$badfilter
||cision.com^$third-party
||ck.page^$third-party
||cmp.radioplay.se^
||cmp.setupcmp.com^$domain=se.azrhymes.com
||cms.catena.media/js/cm-tracking
||cncptx.com^$third-party
||cncpt-central.com^$third-party
||cncpt.dk^$third-party
||collect.breakit.se^
||compado.com^$third-party
||compricer.se^$third-party
||connectio.s3.amazonaws.com/connect-retarget$script
||connect.facebook.net^$domain=friatider.se|fotosidan.se|ng.se|psykologiguiden.se|lektionsbanken.se|lajvo.se|kvinnatillkvinna.se|epochtimes.se|newsner.com|humorbibeln.se|sportbibeln.se|ettgottskratt.se|djurbibeln.se|sillyseason.se|loppi.se|kyrkanstidning.se|tn.se
||connect.nosto.com^*/behav-popup.$script
||consentframework.com^$domain=luleahockeyforum.com|se.moyens.net
||consentmanager.net^$domain=allastudier.se|gbgfotboll.se|stff.se|svenskfotboll.se|coop.se|dagens.se|mobil.se|kamerabild.se|prevent.se|utsidan.se|inpress.com|studentum.se|utbildning.se
||consent.podplay.com^
||converdiant.com^$third-party
||convertbox.com^$third-party
||convertful.com^$third-party
||convertkit.com^$third-party
||conviva.com^$third-party
||cookiebot.com^$domain=ng.se|swedroid.se|bax-shop.se|kurera.se|upplysning.se|mitti.se|circlek.se|findroommate.se|sakochliv.se|polistidningen.se|fokus.se|spraktidningen.se|varden.se|trafiken.nu|energi.se|sverigesnatur.org|kreditrapporten.se|sis.se|accentmagasin.se|allsvenskan.se|superettan.se|alltomarbetsmiljo.se|tco.se|totallyorebro.se|totallystockholm.se|enirobuddy.se|framtid.se|byggfaktadocu.se|husdjur.se|chalmers.se|elinstallatoren.se|ff.se|modernpsykologi.se|qx.se|vatternrundan.se|vvsforum.se|naturvetarna.se|skolporten.se|dust2.se|ehandel.se|byggvarlden.se|varldenidag.se|influens.se|omtanke.today|konsumentmagasinet.se|svenskelitfotboll.se|journalisten.se|fastighetsvarlden.se|jaktjournalen.se|friidrott.se|dagensps.se|vildmarken.se|kyrkanstidning.se|tmf.se|sokbat.se|bilkompaniet.se|driva-eget.se|hv.se|folkhalsomyndigheten.se|dinpsykiskahalsa.se|ekonomifakta.se|hyresbostader.se|rsyd.se|byggforetagen.se|vasterastidning.se|storyhouseegmont.se
||cookiehub.net^$domain=da.se
||cookieinformation.com^$domain=folkofolk.se|dental24.se|vinbanken.se|handelskammarenvarmland.se|enahabo.se|bostadsportal.se
||cookieinfoscript.com^$domain=webbkryss.nu
||cookielaw.org^$domain=cartoonnetwork.se|tv4.se|fotbollskanalen.se|koket.se|flashscore.se|ikea.com|recept.se|manpower.se|mtv.se|natgeotv.com|internetkunskap.se|internetstiftelsen.se|yelp.se|spisa.nu|viaplayradio.se|booli.se|svenskarnaochinternet.se|sv.bab.la|tripadvisor.se|sydkusten.es|livetochdiabetes.se|voister.se|nok.se|motesplatsen.se|thelocal.se|placera.se|infotorgjuridik.se|se.trustpilot.com|travronden.se|travrondenspel.se|hammarbyfotboll.se|pricerunner.se|billetto.se|lidl.se|pwc.se
||cookiepro.com^$domain=birthday.se|djurskyddet.se|havet.nu|svenskfast.se|fiskejournalen.se|upplysning.se
||cookietractor.com^$domain=innebandy.se|orientering.se|pluggakuten.se|munskankarna.se
||cookie-script.com/analytics
||cookie-script.com^$domain=axess.se|dagensjuridik.se|foodfolder.se|arkitektur.se|internetlankar.se|friluftsframjandet.se|lchfarkivet.se|bakasockerfritt.se|handelsradet.se|cirkulation.se
||covatic.io^$third-party
||createsend1.com^$third-party,~image
||createsend.com^$third-party
||curemedia.se^$third-party
||custosgroup.com^$third-party
||cxpublic.com^$third-party
||d1dy2xw1aqg7xq.cloudfront.net/seo_clickin_script
||d1ggib8p3xdn3u.cloudfront.net/script.js
||d1gwclp1pmzk26.cloudfront.net/agile/agile-cloud.js
||d2m8uxg4w7uelx.cloudfront.net/fpa.js
||d2m8uxg4w7uelx.cloudfront.net/fullpageads
||d2qrdklrsxowl2.cloudfront.net/js/hapyak.js
||d9v72urx9pbbc.cloudfront.net/LoadSlotLocator
||d9v72urx9pbbc.cloudfront.net/channel
||d10lumateci472.cloudfront.net/?amuld$script
||d11j2g8hmtmh4u.cloudfront.net/losad
||d11j2g8hmtmh4u.cloudfront.net/loswidget
||d11j2g8hmtmh4u.cloudfront.net/orion
||d11j2g8hmtmh4u.cloudfront.net/tags
||d16fx559zbp759.cloudfront.net/common
||d16fx559zbp759.cloudfront.net/sites
||d24rtvkqjwgutp.cloudfront.net/*yb.js
||d31djwpx7pcvsr.cloudfront.net/production/*/js/segment.js
||d2189b0dij3l7v.cloudfront.net/p/$domain=tv4play.se|tv4.se|fotbollskanalen.se|koket.se
||dackpartner-web.s3.amazonaws.com^$third-party
||deals.innocode.no^$third-party
||delivery.youplay.se/api/player_metrics?
||delivery.youplay.se/report?$image
||destination.se^$third-party
||didomi.nwtmedia.se^
||digitaliseringsinitiativet.se^
||digitaloceanspaces.com/ethical.min.js
||dinbilgaranti.se^
||distansarbete.com^
||diu127fbe6pn6.cloudfront.net^*/ga-universal.html
||doktor-se.onelink.me^$image
||driftt.com^$third-party
||drift.com^$third-party
||dsms0mj1bbhn4.cloudfront.net/assets/pub/shareaholic.$script
||dspk.kindredplc.com/renderImage.aspx$image
||eacdn.com/TrafficOpt/$script
||easyweb.se/stats/$image
||ebbot.eu/api/widget/analytics
||ecomm.events/i.js
||ekonomifakta.se/monitoring
||elfsight.com/events/views
||embed.lpcontent.net/leadboxes$script
||embed.viaplay.com/*autoplay=true$frame,removeparam=autoplay
||embi-media.com^$third-party
||emg-services.net/public/scripts/bundles/emg-desktop
||emg-services.net/public/scripts/bundles/emg-dfp
||emotorsport.se/ans/$image
||eniro.se/scoop.js
||entainpartners.com^$third-party
||episerver.net/*/epi-util/find.js
||es.loppi.se^
||etc.nu/ethical.min.js
||eugamblers.org^$third-party
||europe-west1-bonnier-big-data.cloudfunctions.net^$third-party
||eu-north-1.amazonaws.com/*images/*Banner
||events.forzasys.com/get.min.js
||evertiq.se/bimg/
||evidon.com^$third-party,domain=fasting.nu
||evt-api.ntm.eu/api/*/datacollector
||execute-api.eu-west-1.amazonaws.com/live/analytics
||existenz.se/img/o/
||exitintel.com^$third-party
||expekt.se^$third-party
||extellio.com^$third-party
||external.reseguiden.se/offer
||facebook.com/plugins/share_button$third-party
||facebook.com^*/plugins/like$third-party
||fakturino.se^$third-party
||familjehemsbanken.se/api/partners
||famobi.com/play/hit/
||fastout.com/analytics
||fasttrack.webstream.dk/statistik
||feedblitz.com^$third-party
||feeds.feedburner.com^$image
||feed.mikle.com^$third-party,domain=ekonominyheter.se
||filasverigese.com^
||fila.com.se^
||files.cdn.spilcloud.com/pb/$script
||filmtopp.se/upload/*/annons$image
||findit.fi/js/prebid
||flashback.org/rlog.php
||flirtmatch.se^
||fodertipset.se/cookie-info
||folkspel.se^$third-party
||footjoygolfskorrea.com.se^
||forms.hsforms.com^*/counters.$image
||forum.odla.nu/js/bonnier.js
||fotboll.com/*casino$image
||fraagesport.com^
||freewheel-mtgx-tv.akamaized.net^$media
||freyanews.com^*/tracker$script
||fritiden.se/js/cookiealert-standalone.js
||funnelytics.io^$third-party
||gamblersrules.com^$third-party
||gamblingsyndication.com^$third-party
||gamedistribution.com/libs/gd/analytics
||gamereactor.se/ads/
||gamereactor.se/exclusive.json
||gamesglue.com/js/gameanalytics/GameAnalytics
||gatekeeperconsent.com^$domain=hemmanytt.se|svenskaorduttryck.se|wernamaten.se|sanghafte.se
||getanewsletter.com/js-forms-assets/popups.js
||getlevelten.com^$third-party
||getsitecontrol.com^$third-party
||girohjalm.com.se^
||glitnoraffiliates.com^$third-party
||gnuheter.com/creeper/image
||googletagmanager.com^$important,domain=tradera.com|xxl.se|prisjakt.nu
||google-analytics.com^$important,domain=aftonbladet.se|tradera.com|xxl.se
||gopeach.se^$third-party
||gravito.net^$domain=hitta.se|gp.se|bohuslaningen.se|stromstadstidning.se|markposten.se|harrydaposten.se|partilletidning.se|sttidningen.se|molndalsposten.se|kungalvsposten.se|kungsbackaposten.se|alingsastidning.se|ttela.se|hallandsposten.se|hn.se|mellerudsnyheter.se
||grillbloggen.nu/media/com_rstbox/js/engagebox.js
||growthbook.io^$domain=allas.se|elle.se|femina.se|hant.se|mabra.com|residencemagazine.se|svenskdam.se|motherhood.se
||gstatic.com/partners/badge$subdocument
||gtm.ekonomifakta.se^
||gtm.findroommate.dk^
||guesssverige.com.se^
||gymshark-sweden.com.se^
||hajper.com^$third-party
||happygreen.se^$third-party
||hapyak.com^$third-party
||harmonious-station-to-station.podplay.com/script.js
||hastnet.se/adtech
||hejauppsala.com/*banner$image
||helix.svt.se/events
||helloreco.com^$third-party
||heroaffiliates.com^$third-party
||herokuapp.com/visit?$image
||hittahem.se^$third-party
||hltv.org/js/ht.$domain=dust2.se
||hockeysnack.com/pagespeed_static/1.$image
||hoomemakleri.se^$third-party
||humorbrevet.se/externa_bilder
||iconosquare.com^$third-party
||ifragasatt.se/stats/
||images-ads.aland.com^
||images.woo.a2d.tv/creative_assets$image,domain=tv4play.se|tv4.se|fotbollskanalen.se|koket.se
||imasdk.googleapis.com/js/sdkloader/ima3.js$script,redirect=google-ima.js,important,domain=screen9.com|atl.nu
||imgix.net^*/analytics.$script
||imgsct.cookiebot.com/1.gif
||img.upsales.com/*/visit$script,important
||imp.laget.se^
||inboxads.com^$third-party
||inmobi.com^$domain=alltomelbil.se|rikatillsammans.se|egoinas.se|land.se|moviezine.se|travelnews.se|varldenshaftigaste.se|merinfo.se|foreca.se|matklubben.se|reseguiden.se|newsner.com|humorbibeln.se|sportbibeln.se|ettgottskratt.se|djurbibeln.se|laget.se|byrum.se|sportlovin.se|receptfavoriter.se|forni.se|kimura.se|cornucopia.se|norrahalland.se|elevspel.se|finanstid.se|tittapavideon.se|motormagasinet.se|food-supply.se|dagenshandel.se|plastnet.se|habit.se|woodnet.se|foodnet.se|transportnet.se|processnet.se|packnet.se|verkstaderna.se|medtechmagazine.se|recyclingnet.se|rt-forum.se|uochd.se|lifesciencesweden.se|fri-kopenskap.se|cleannet.se|metal-supply.se|framtidensbygg.se|entreprenad.com|mykitchenstories.se|cancelculture.se|mytaste.se|findit.se|lchfarkivet.se|brinkenbakar.se|foretagande.se|fotbolltransfers.com|affarsvarlden.se|villalivet.se|branschaktuellt.se|nordic.ign.com|fragbite.se|lindasbakskola.se|jennysmatblogg.nu|filippoon.se|lesscarbs.se|eniro.se|matspar.se|xnytt.se|alltomkungligt.se|swehockey.se|vackertvader.se|newly.se|nyheter2.se
||insertcoin.se^$third-party
||insplanet.com^$third-party
||instaforex.com^$third-party
||instiengage.com^$domain=stoppapressarna.se
||intagme.com^$third-party
||interactiveads.ai^$third-party
||internetmedicin.se/log.php
||investerarbrevet.se^$third-party
||iphonecasinon.com^$third-party
||isgprivacy.cbsi.com^$domain=nickelodeon.se
||jajja.com^$third-party
||jenkler.se^$domain=uex.se
||jitsu.com/p.js
||jobba-hemifran.com^
||jobb.blocket.se/blocket_puff.html
||jobb.blocket.se^*/tracker.js
||jobb.blocket.se^*/xtcore.min.js
||jobtip.se^$domain=shortcut.se
||jst.ai^$third-party
||js.adsaga.se^$third-party
||js.evtr.nordiskemedier.dk^
||js.hs-banner.com^
||js.rating-widget.com/external
||juicer.io/api/page_views
||jwpcdn.com/player/plugins/inference/
||jwpcdn.com/player/*/bidding.js$domain=allas.se|elle.se|femina.se|hant.se|mabra.com|residencemagazine.se|svenskdam.se|motherhood.se|recept.se
||jwplayer.com/*/advertising$domain=allas.se|elle.se|femina.se|hant.se|mabra.com|residencemagazine.se|svenskdam.se|motherhood.se
||k5a.io^$script,redirect=noop.js,domain=tv2.no
||kajabi-cdn.com^$domain=nillaskitchen.com
||kalender.se/analytics
||kamrat.com/js/cookiescript
||kayak.xno.se^$script
||keenstockholm.com.se^
||kingsizemag.se/content/
||kingsizemag.se/kingrev.php
||kingsumo.com^$third-party
||klaviyo.com^$third-party,domain=~kmail-lists.com|~myklpages.com
||kolozzeum.com/forum/kollos$script
||konzilo.com/mtc.js
||konzilo.net/mtc.js
||kortio.se^$third-party
||kritiker.se/js/gdpr.js
||kundvisaren.se^$third-party
||kyrkanstidning.se/firstvisit$xhr,empty
||laget.se^*/retarget.js
||lajvo.se/addImpression
||lanapengar.expressen.se^
||lantbruksnet.se/files/reklan/
||lantbruksnytt.se/includes/$subdocument
||laromedia.se/Annonssystem/
||lasso.link^$third-party
||leadconnect.ipmaxi.se^$third-party
||leadenhancer.com^$third-party
||leazard.io^$domain=varmepumpsforum.com
||libring.com^$third-party
||lib.atomik.vip/loader.min.js
||lifeofsvea.se/production/borka/
||lifeofsvea.se/production/losjs/
||lifestyle.expressen.se^$subdocument
||likebtn.com^$third-party
||liveagent.se/scripts/track
||live-tag.creatopy.net^$third-party
||ljudoljus.net/images/banner/
||logsnag.com^$third-party
||logs.sesamy.com/events
||lokalguiden.se/magasinet/banner
||lok.se/pic/sponsor/
||longchampstockholm.com.se^
||lookaside.fbsbx.com/lookaside/crawler/
||look.ufinkln.com^
||look.utndln.com^$all
||lwadm.com^$important,domain=sydostran.se
||lwcdn.com/vendor/ima.min.js$script
||lystra.se^$third-party
||m1.analytics.sitevision-cloud.se^
||mailchimp.com^*/popup$script
||mailerlite.com/*/universal/*popups.js
||mailerlite.com^$third-party,domain=vandringsguiden.se|flm.nu
||mailmunch.co^$third-party,domain=affarsstaden.se|enkelteknik.se
||mailmunch.co^*/scrollbox$script
||makeinfluence.com^$third-party
||manatee.dk^$third-party
||manatee.io^$third-party
||marfeelcache.com^$third-party
||marketo.com^$third-party
||masture.mobi^
||matchads.net^$third-party
||matchesfashion.com^*/ExternalBanners
||matorama.se^$csp=img-src 'self' *.wordpress.com *.wp.com *.gravatar.com
||maxetise.net^$script,redirect-rule=noop.js,domain=feber.se|tjock.se
||mcgtrack.herokuapp.com^$third-party
||mediacreeper.com/image$image,redirect=32x32.png
||mediacreeper.se/image$image,redirect=32x32.png
||mediakraft.se^$third-party
||mediaserver.gvcaffiliates.com.cdn.cloudflare.net^
||media.arto.se/*annons$image,domain=natursidan.se
||media.dagensps.se/*banner$image
||media.golfbladet.se/*banner
||media.jw-it.se/b/$image
||media.jw-it.se/getip.php
||mediekompaniet.com^$third-party
||meltwater.com^$third-party
||metalcentral.net/images/*banner
||metapic.se^$third-party
||metromode.se/widget/club/
||mikz.com^$third-party
||miljomat.se/annonser
||missaffiliate.com^$third-party
||misssite.com/*/published-site-analytics.js
||mis.se/count/
||mitti.se/agstatistics-
||mitti.se/click-
||mogenromantik.com^
||momondo.se/*gtm/
||mraffiliate.com^$third-party
||mtpc.se^$third-party
||mtst.io/js/mtst.js
||multibrandaffiliates.com^$third-party
||myadmessenger.com^$third-party
||mymediaindex.com^$third-party
||narkive.se/ajax/Telem
||network-n.com^$third-party
||newsharecounts.*.amazonaws.com/nsc.js
||newstag.com/t/e$xmlhttprequest
||newstats.blogg.se^
||ng.se/nodecounter/
||nichehuset.dk^$third-party
||nitroscripts.com^
||nitroz.se/banners.min.js
||nordiskemedier.dk/banner/
||nordiskemedier.dk/bnr/
||nordiskemedier.dk/remodal$script
||nordiskskog.se/dynamic/serve.php
||norstatsurveys.com^$third-party
||notedmedia.se/pixel/
||nouw-ms-blog.azurewebsites.net/api/blogstatistic
||nouw.com/api/campaignpost
||nouw.com/api/postimpression
||nouw.com/api/postview
||nouw.com/campaignpost/reg/
||nuance.com/tagserver/logging
||nucleusanalytics.io^$third-party
||nyheteridag.se/ads/
||nyhetersto.se/webpushr-sw
||oas.*.se/om/$script
||obj.fotosidan.se/obj/pa/$image
||offer-go.com^$third-party
||onesignal.com^$domain=samnytt.se|battrestadsdel.se|beernews.se|ungdomsfotboll.se|rabattsok.se|1x2.se|cannabis.se|dackavisen.se|driva-eget.se|skogsaktuellt.se|maskinbladet.se|entreprenadaktuellt.se|ja.se|newsner.com|humorbibeln.se|sportbibeln.se|ettgottskratt.se|djurbibeln.se|finanstid.se|fokus.se|gasetten.se|fotbollsthlm.se|macken.xyz|naringslivetvgl.se|dalarnasaffarer.se|stockholmsaffarer.se|jamtlandsaffarer.se|hallandsnaringsliv.se|sjuharadsnaringsliv.se|netflixguiden.se|nyadagbladet.se|oskarshamns-nytt.se|swebbtv.se|thepattayanews.se|vaken.se|aktieskolan.se|fastighetsvarlden.se|mcparken.se|gaffa.se|alltomnorrtalje.se|morotsliv.com|it-finans.se|it-halsa.se|it-kanalen.se|it-pedagogen.se|it-retail.se|skaneplus.se|mittforetag.com
||onetrust.com^$third-party,domain=lantmannen.se
||online.bookvisit.com^$third-party,domain=campingsverige.se
||online.swedbank.se.swedd.$document
||onrender.com/tracker.js
||open-analytics.se^$third-party
||opinionstage.com/assets/autoengage.$script
||optmn.cloud/hb/
||optnmnstr.com^$third-party
||opulens.se^$csp=worker-src 'none'
||organicfruitapps.com/analytics
||owa.agriprim.se^
||pafpartners.com^$third-party
||palmangelssverige.com.se^
||pcf.tdscd.com^
||peertube.se^$frame,redirect=click2load.html,domain=nordiskradio.se
||pensiono.se.$subdocument
||pensiono.se^$third-party
||petrk.com^$third-party
||pheegoab.click^
||piano.io^$domain=thelocal.se|illvet.se|iform.se|varldenshistoria.se|popularhistoria.se|dagen.se|gds.se|slakthistoria.se|digitalfotoforalla.se
||pingback.issuu.com/ping
||pipedrive.com^*/statistics/seen
||pixel.bet^$third-party
||pixel.playbuzz.com^
||pji.nu/libs/pjpixel
||pji.nu^$third-party,domain=minhembio.com|ljudochbild.se
||platform.linkedin.com^$third-party
||platform.tumblr.com/*/share.js$third-party
||platssajten.se^$third-party
||plausible.io^$script,redirect-rule=noop.js,domain=feber.se|tjock.se
||plausible.webfokus.no^$third-party
||player.vimeo.com^$frame,redirect=click2load.html,domain=breakit.se
||pliing.com^$third-party
||plowking.mecenat.com^
||pm.azerioncircle.com^
||podcasts.nu/adbg.svg
||poddtoppen.se/api/ad?
||pomu.se/api/ads.json
||pomu.se/games/visit/
||portalhc.com^$third-party
||pricerunner.com/publisher-widgets$third-party
||prisjakt-a.$third-party,domain=~prisjakt.nu|~prisjakt.no|~pricespy.co.uk|~ledenicheur.fr|~prisjagt.dk|~pricespy.co.nz|~hintaopas.fi
||prisjakt.nu^$third-party
||prismic.io/prismic-toolbar$domain=alltomarbetsmiljo.se
||privacypolicies.com^$domain=fl-net.se
||privacy-center.org^$domain=180.se|agriaffaires.se|truckscorner.se|machineryzone.se|stegforhalsa.se|netdoktor.se|netdoktorpro.se|news55.se|hastnet.se
||privacy-mgmt.com^$domain=radio.se|dagenstv.com|kolla.tv|computersweden.se|woxikon.se|kokaihop.se|dagen.se|filmtopp.se|upday.com|gaffa.se
||prod.uidapi.com^$domain=tittapavideon.se
||proff.se^$third-party
||proxyas.com^$third-party
||prvcy.vkmedia.se^
||prylguiden.expressen.se^
||ptm.flowplayer.com^*/display$xmlhttprequest
||ptm.flowplayer.com^*/ping$xmlhttprequest
||ptm.flowplayer.com^*/view$xmlhttprequest
||pt.dwcdn.net/*/datawrapper.gif
||pushcrew.com^$third-party
||pushnice.com^
||pushpushgo.com^$third-party
||pushwhy.com^
||pxl.host^$third-party
||qimtek.se^$third-party
||quantcast.com^$domain=flashback.org|babyhjalp.se|nyadagbladet.se|enkelteknik.se|travelgrip.se|samnytt.se|nyteknik.se|lag-avtal.se|arbetarskydd.se|leta.se|motivation.se|sporttv.nu|goforfit.se|expo.se|poddtoppen.se|langd.se|doon.se|garaget.org|nouw.com|listor.se
||qx.se/view.php$image
||rabble-res.cloudinary.com^$third-party
||radio.se/iomm
||ramses.nu^$third-party
||raygun.io^$domain=koket.se
||reaktion.se^$third-party
||recirculation.spot.im^$third-party
||reco.se/widget/analytics
||reddit.com/static/button$third-party
||redeal.se^$third-party
||referralhero.com^$third-party
||rejsa.nu/ann$image
||rekai.se^$third-party,domain=folkpool.se
||rektek.se/widget/extraexposurejobs$third-party
||rek.ai^$third-party,domain=ng.se
||researchonline.se^$third-party
||reseguiden.se^$third-party
||reseguiden.se^*/google-tag
||resources.blogblog.com^*/paging_dot.$image
||resultify.com^$third-party
||resultify.se^$third-party
||res.cloudinary.com/internetmedicin/image/*/friends/
||res.se/js/ad.js
||revrelations.com^$third-party
||richmediastudio.com^$third-party
||riedta.com^$third-party
||routy.app^$third-party
||royapp.com^$third-party
||rpofsweden.com^
||rpofsweden.se^
||runtnc.net^
||salesiq.zoho.com/widget$domain=seodesign.se
||salesmanago.pl/api/push/notification$domain=aikfotboll.se
||salesmanago.pl/*popup$domain=land.se
||sales.agriprim.com/Banners
||sannsyn.com^$third-party
||sa.svenskalag.se/*/__tm.gif
||scandicpartners.se^$third-party
||schibsted.com/pulse$domain=aftonbladet.se
||script.e-space.se^$third-party
||sdk.mrf.io/statics/marfeel-sdk
||sdk.pulse.schibsted.com^$script,domain=aftonbladet.se|omni.se|omniekonomi.se|svd.se|prisjakt.nu
||seenthis.se^$third-party
||selectofmychoices.com^
||sellingsimplified.net^$third-party
||seonify.com^$third-party
||servg1.net^$third-party
||service.force.com^$domain=allabolag.se
||se-affiliate-gallery.aws.aller.com^
||shareaholic.com^$third-party
||shareaholic.net^$third-party
||sharedcount.com^$third-party
||sharethis.com^$third-party
||sitegainer.com/jsinsert/*/sitegainer$third-party
||skk.se/TSPD/
||skogsforum.pro/analytics
||skogsforum.se/async
||skogsforum.se^$csp=worker-src 'none'
||sleeknote.com^$third-party
||smartstats.kla.tv^
||snapwidget.com/images/snapwidget_ad
||snt-matrix-app.herokuapp.com^*/user-tracking
||solidtango.com^*/player_statistics$image
||spania.no^$third-party
||spelguiden.samnytt.se^
||spelhubben.se/?_dnembed$script
||spel.expressen.se^
||sporttv.nu/images/BetLogos
||sporttv.nu/images/sponsor/
||sporttv.nu/js/partners
||sprida.se^$third-party
||sprinkletxt.com^$third-party
||sp.tinymce.com^$image
||srvrtools.com/r/p.html?$subdocument
||srvrtools.com/t.js?
||stackpathcdn.com^*/shrMain$script
||stadiumstage.com^$third-party
||stallet.se/scripts/bx-abd.js
||static.hupso.com/share/js/counters.js
||statisticplatform.com^$third-party
||stats2.ehandel.se^
||stats.blogg.se^$image
||stats.docu.info^
||stats.easyweb.se^$third-party
||stats.ehandel.se^
||stats.helsingborg.se^
||stats.jibber.social^
||stats.playoncenter.com^
||stats.poddtoppen.se^
||stats.proff.se^
||stats.tipser.com^$xmlhttprequest
||stat.modette.se^
||stayfriends.de/metatag
||step.dk^$third-party
||stm.eniro.se^
||stockholmtarot.se^$third-party
||storage.googleapis.com/didna$third-party
||storymedia.se^$third-party
||streamio.com/api/*/stats$xmlhttprequest
||studads.com^$third-party
||suntana.se^$third-party
||susnet.*/susnetstat.js$script
||svd.se/api/dr-edition-teasers
||svd.se/api/live-ads/
||svenskafans.com/menu-logo/bottom
||sv.picmix.com/sw.js
||sv.picmix.com^$csp=worker-src 'none'
||s.arclk.net/tr?$all
||tally.so^$domain=tranakampsport.se
||tc.hometogo.net^$image
||telemetry.bambuser.io^
||tibaco.net/scripts/tws.js
||toolcontentcloud.com/*/asjs$domain=bredband.se
||top100ruokablogit.com^$third-party
||topblogarea.se/tracker
||toppmarkensverige.com^
||tourn.co^$third-party
||tourn.se^$third-party
||tracking.bonnier.news^
||tracking.fasab6f.se^
||track.intersport.se^
||track.postkodlotteriet.se^
||track.yetric.app^
||tradehouse.media^$third-party
||travellink.se/marketing-channel
||travronden.se/monitoring
||travtjansten.se^$third-party
||trckr*.nordiskemedier.dk^
||tripadvisor.se/PVLog
||tripadvisor.se/data/*/rum
||tripadvisor.se^$csp=worker-src 'none'
||tr.apsisforms.com^$third-party
||turistmal.se/js/popup-controller.js
||tv4.video-tracking.a2d.tv/anonymous/event
||tvmatchen.nu/plugins/splash-redirector
||tvmatchen.nu^*/smartbanner
||tvm-tv4-freewheel.akamaized.net^
||twingly.com^$third-party
||twitcount.com^$third-party
||t.atmng.io^
||t.elasticsuite.io^$third-party
||t.fml.rip^$third-party
||t.raptorsmartadvisor.com^$image
||ubembed.com^$third-party
||ues.vk.se^*/events
||ufinkln.com/offer?prod$popup
||umami.nordiskehandel.cloud^
||upsales.com^$third-party
||usabil.nu/media/*/casino$image
||usefathom.com^$domain=fz.se|sweclockers.com
||usercentrics.eu/1.gif
||usercentrics.eu/uct?$image
||usercentrics.eu^$domain=hemnet.se|kantarsifo.se|foretagarna.se
||userneeds.com^$third-party
||valentinosverige.com^
||vejaskor.com.se^
||vejasskor.com^
||viadata.store^$third-party
||viagogo.se^
||viforetag.se^$third-party
||vinguiden.com^$third-party
||viralize.tv/t-bid
||viralize.tv^$domain=tyda.se
||vovve.net/i/sponsorer
||voyager-widgets.aftonbladet.se/widgets/sports
||walls.io^$domain=svensktgolfforum.se
||wayke.se^$third-party,domain=siljannews.se
||wct-1.com^$third-party
||wct-2.com^$third-party
||webbannons.ntm.eu^$subdocument
||webbjobb.io^*/abb-$script
||webformscr.com/apps/fc3/build/default-handler.js
||webpower.eu^$third-party
||webpushs.com^$third-party
||websta.me^$third-party
||widgets.bonniernewslifestyle.se^$subdocument
||widgets.getpocket.com^$third-party
||widgets.jobtechdev.se^$third-party
||widget.getyourguide.com^$third-party
||widget.matklubben.*/tracker
||widget.mytaste.*/blogcounter
||widget.playoncenter.com/newplayer/js/pb_$script,redirect=noop.js
||wisepops.com^$third-party
||wishpond.net^$third-party
||woomio.com/assets/js/analytics
||workhaus.se^$third-party
||yelp.se/sit_rep
||yieldwrapper.com^$third-party
||youbora.com^*/sp.min.js$important,domain=aftonbladet.se|svd.se|livsstil.se|godare.se|tv.nu
||youtube.com/embed$frame,redirect=click2load.html,domain=ordfrontmagasin.se
||youtube.com/embed/*autoplay$subdocument,removeparam=autoplay,domain=kritiker.se
||ysektionen.se/media/uploads/*banner$image
||znaptag-tags-se.s3.amazonaws.com^$script
||zoho.com/hub/js/WebsiteAutomation.js$third-party
||zummycloud.com^$third-party
||zummy.io^$third-party
!#if env_chromium
||fast.fonts.com/t/1.css
||fast.fonts.net/t/1.css
||fast.fonts.net/lt/1.css
!#endif
!#if env_mobile
##.banner--mobiletoppanorama
##.mobile-homepage-ad
##.mobile-main-ad
##.mobil-annons
###mobile-banner-top
###mobile-banner-after-content
###mobile-banner-bottom
##div.mobile-ads-wrapper
##div.top-mobile-ad
##div.mobileads
##div.big-mobile-ads
##div#topBannerMobile
!#endif
!#if !env_chromium
||fast.fonts.net/*/1.css$domain=arkitekt.se|axess.se|diabetes.se|sverigeslarare.se|ljuskultur.se|electronic.se
branschkoll.se,rocknytt.net,upphandling24.se,kimura.se,datormagazin.se,villalivet.se,classicmotor.se,tidningenhalsa.se,husohem.se,guiden.se,nyadagbladet.se,enkelteknik.se,stoppapressarna.se##^script[id^="advanced-ads"]
branschkoll.se,rocknytt.net,upphandling24.se,kimura.se,datormagazin.se,villalivet.se,classicmotor.se,tidningenhalsa.se,husohem.se,guiden.se,nyadagbladet.se,enkelteknik.se##^script[id^="advanced_ads"]
branschkoll.se,rocknytt.net,upphandling24.se,kimura.se,datormagazin.se,villalivet.se,classicmotor.se,tidningenhalsa.se,husohem.se,guiden.se,nyadagbladet.se,enkelteknik.se##^script[id^="advads"]
branschkoll.se,rocknytt.net,upphandling24.se,kimura.se,datormagazin.se,villalivet.se,polistidningen.se,densistavilan.se,classicmotor.se,tidningenhalsa.se,husohem.se,guiden.se,nyadagbladet.se,enkelteknik.se##^script:has-text(advanced_ads)
branschkoll.se,rocknytt.net,upphandling24.se,kimura.se,datormagazin.se,villalivet.se,polistidningen.se,densistavilan.se,classicmotor.se,tidningenhalsa.se,husohem.se,guiden.se,nyadagbladet.se,enkelteknik.se##^script:has-text(advads)
stoppapressarna.se##^script[data-src*="advads"]
temadagar.se,lchfarkivet.se,wernamaten.se,sanghafte.se##^script:has-text(__ez)
svt.se###nyh_a11y-primary-navigation-list:style(float:unset!important;)
!#endif
!#if !env_mobile
/assets/js/modules/plugins/smoothPageScroll
/rokophoto-lite/js/SmoothScroll
/wp-enqueue/*smoothscroll
/themes/*/js/smoothscroll
/jquery.smoothwheel/*
/tapatalkdetect$script,1p
/themes/Jaz/inc/js/*nicescroll
/smart-app-banner*/banner.js
lundagard.se,boktugg.se,morotsliv.com,affarsstaden.se,kurera.se,nyfiknainvesterare.se##+js(aeld, wheel)
home2tiny.se##+js(aeld, /mousewheel|DOMMouseScroll/, smoothScrollEvent)
!#endif


! Title: Hide YouTube Shorts
! Description: Hide all traces of YouTube shorts videos on YouTube
! Version: 1.9.0
! Last modified: 2024-02-17 11:55
! Expires: 2 weeks (update frequency)
! Homepage: https://github.com/gijsdev/ublock-hide-yt-shorts
! License: https://github.com/gijsdev/ublock-hide-yt-shorts/blob/master/LICENSE.md

! Remove empty spaces in grid
www.youtube.com##ytd-rich-grid-row,#contents.ytd-rich-grid-row:style(display: contents !important)

! Hide all videos containing the phrase "#shorts"
www.youtube.com##ytd-grid-video-renderer:has(#video-title:has-text(/(^| )#Shorts?( |$)/i))
www.youtube.com##ytd-rich-item-renderer:has(#video-title:has-text(/(^| )#Shorts?( |$)/i))

! Hide all videos with the shorts indicator on the thumbnail
www.youtube.com##ytd-grid-video-renderer:has([overlay-style="SHORTS"])
www.youtube.com##ytd-rich-item-renderer:has([overlay-style="SHORTS"])
www.youtube.com##ytd-video-renderer:has([overlay-style="SHORTS"])
www.youtube.com##ytd-item-section-renderer.ytd-section-list-renderer[page-subtype="subscriptions"]:has(ytd-video-renderer:has([overlay-style="SHORTS"]))

! Hide shorts button in sidebar
www.youtube.com##ytd-guide-entry-renderer:has(yt-formatted-string:has-text(/^Shorts$/i))
! Tablet resolution
www.youtube.com##ytd-mini-guide-entry-renderer:has(.title:has-text(/^Shorts$/i))

! Hide shorts section on homepage
www.youtube.com##ytd-rich-section-renderer:has(#title:has-text(/(^| )Shorts( |$)/i))
www.youtube.com##ytd-reel-shelf-renderer:has(.ytd-reel-shelf-renderer:has-text(/(^| )Shorts( |$)/i))

! Hide shorts tab on channel pages`
! Old style
www.youtube.com##tp-yt-paper-tab:has(.tp-yt-paper-tab:has-text(Shorts))
! New style (2023-10)
www.youtube.com##yt-tab-shape:has-text(/^Shorts$/)

! Hide short remixes in video descriptions
www.youtube.com##ytd-reel-shelf-renderer.ytd-structured-description-content-renderer:has-text(/^Shorts remixing this video$/i)

! Hide shorts category on homepage and search pages
www.youtube.com##yt-chip-cloud-chip-renderer:has(yt-formatted-string:has-text(/^Shorts$/i))

!!! MOBILE !!!

! Hide all videos in home feed containing the phrase "#shorts"
www.youtube.com##ytm-rich-item-renderer:has(#video-title:has-text(/(^| )#Shorts?( |$)/i))

! Hide all videos in subscription feed containing the phrase "#shorts"
m.youtube.com##ytm-item-section-renderer:has(#video-title:has-text(/(^| )#Shorts?( |$)/i))

! Hide shorts button in the bottom navigation bar
m.youtube.com##ytm-pivot-bar-item-renderer:has(.pivot-shorts)

! Hide all videos with the shorts indicator on the thumbnail
m.youtube.com##ytm-video-with-context-renderer:has([data-style="SHORTS"])

! Hide shorts sections
m.youtube.com##ytm-rich-section-renderer:has(.reel-shelf-title-wrapper .yt-core-attributed-string:has-text(/(^| )Shorts( |$)/i))
m.youtube.com##ytm-reel-shelf-renderer.item:has(.reel-shelf-title-wrapper .yt-core-attributed-string:has-text(/(^| )Shorts( |$)/i))

! Hide shorts tab on channel pages
! Old style
m.youtube.com##.single-column-browse-results-tabs>a:has-text(Shorts)
! New style (2023-10)
m.youtube.com##yt-tab-shape:has-text(/^Shorts$/)

! Hide short remixes in video descriptions
m.youtube.com##ytm-reel-shelf-renderer:has(.reel-shelf-title-wrapper .yt-core-attributed-string:has-text(/^Shorts remixing this video$/i))

! Hide shorts category on homepage
m.youtube.com##ytm-chip-cloud-chip-renderer:has(.yt-core-attributed-string:has-text(/^Shorts$/i))

! Block .zip and .mov domains
||zip^
||mov^
```

### Swedish filter

```
! Title: Frellwit's Swedish Filter
! Last updated: Tue, 16 Jul 2024 07:57:28 +0000
! Expires: 5 days
! Diff-Path: patches/2024.7.16.477.patch#swefilter
! Diff-Expires: 24 hours
! Description: A filter for uBlock Origin that aims to remove regional Swedish ads, tracking, annoyances, scams + badware, and unnecessary bloat.
! Homepage: https://github.com/lassekongo83/Frellwits-filter-lists
! License: https://github.com/lassekongo83/Frellwits-filter-lists/blob/master/LICENSE
! *** swefilter:Frellwits-Swedish-Filter.txt ***
.ads-gdprlock
.ax/ad/
.ax/images/banners/
.com/annonsmaterial/
.com/annons.$script,subdocument
.com/misc/loada.js
.html$subdocument,domain=flygtorget.se
.js?cb$domain=hemmanytt.se
.js?gcb$domain=hemmanytt.se
.nu/annons/
.nu/banner/
.nu/files/banner/
.nu/gfx/banner/
.nu/prebid$script
.php?annonsid=$image
.se/AdPlugins/
.se/Banners/
.se/Logger?
.se/Media/Banners/
.se/Static/banners/
.se/adson/$subdocument
.se/adstart.php
.se/advertisement_script
.se/advert$subdocument
.se/adx.js
.se/ad-delivery/
.se/ad/AdSpaceBlock/
.se/annons.$script,subdocument
.se/annons/$domain=~blocket.se
.se/assets/scripts/prebid
.se/banner.stat?
.se/banner/
.se/bildbank/banners/
.se/bilder/banners/
.se/blogcounter/image?
.se/common/js/tracking/
.se/counter/
.se/custom/ad/
.se/fightodds.plugin/fightodds.plugin.$script
.se/files/ads/$image
.se/files/annons/$image
.se/getBannerImage
.se/globalassets/banners/
.se/images/banners/
.se/images/banner/
.se/img/banners/
.se/js/ga.js|
.se/load-ads/
.se/logger.
.se/log/?
.se/makebnr.asp?
.se/misc/loada.js
.se/native?noBurtProfiles
.se/nonsec/banner/
.se/portalen-stats/register-view
.se/prebid$script
.se/pres/bnrs/$image
.se/revive/www/
.se/scripts/google-funding-choices.js
.se/sponsored/$image
.se/track/t.php?
.se/uploads/banners/
.se/uploads/images/banners/
.se/upload/annons/
.se/upload/_ads/
.se/wdg/tracking
.se/wdg/vda-active
.se/wp-content/banners/
.se/wp-content/uploads/_banners/
.se/xhr/add-impression/
.se/*/gillkom?$xmlhttprequest
.se/*/nativeadvertising/
.se/*/postkoll?$xmlhttprequest
.se/_Banners/
7an.se##.field--name-field-ad-banner-image
8sidor.se###cookie-banner
56kilo.se##.code-block:has(.shop-page-wp-grid)
56kilo.se##.featured-area, .awac-wrapper
56kilo.se##.penci-single-block[data-current-url*="cbd"]:has(a[href*="?ref="])
99.teknikveckan.se##.carousel-item-link:has-text(Annons:)
99.teknikveckan.se##.page-gutter.left, .page-gutter.right, [id^="bbPrisjakt"]
180.se##[class*="top-ad-"]
2000tv.se###bannerbox
Mobile-banner$image,domain=bokadirekt.se
accentmagasin.se##+js(nostif, n.modal)
adecco.se,ica.se,apotekhjartat.se,tele2.se###onetrust-consent-sdk
advokaten.se##.cookieconsent-optin-marketing
affarerinorr.se##a[href^="/nyheter/native-artiklar/"]
affarsstaden.se##+js(acs, jQuery, adblockdetect)
affarsvarlden.se##.article-tag-header:has-text(/Annons/i):upward(article)
affarsvarlden.se##.cookies-wrap, .Modal, .article-list-item--native, .advert-notice-box, .native-popup, .takeover-wrap, .native-notice-box, .darwin--content
aftonbladet.se##article[class^="article-wrapper"] ~ div:has-text(ANNONS)
aftonbladet.se##aside > div:has(h2:has-text(/^annons/i))
aftonbladet.se##a:has-text(Kommersiell text, innehåller annonslänkar)
aftonbladet.se##a[href^="https://kampanj."]:upward(1):not(section):not(div[class^="article-wrapper"])
aftonbladet.se##div[class^="css-"]:has([data-ad-subtype="mega"])
aftonbladet.se##main > section > div:first-child:matches-css(box-shadow: rgba(0, 0, 0, 0.2) 0px 0px 24px 0px)
aftonbladet.se##main > section > div[class^="css-"]:first-child:has(img[src*="closeButton"])
aftonbladet.se##p:has-text(/^PRESENTERAS AV$/):upward(1)
aftonbladet.se##section > div:has(h2:has-text(/^annons/i))
aftonbladet.se##span:has-text(/^annons/i):upward(a)
aftonbladet.se##strong:has-text(/ANNONS/i):upward(p)
aftonbladet.se###main > div > div > div:has(h2:has-text(/^annons/i))
aftonbladet.se###megaAd-placeholder, #superright-side, a[href*="/casinoguide"], [id^="adPlacement"], a[href^="https://kampanj.aftonbladet"], a[href*="/rabattkod"][data-test-tag="internal-link"], a[href^="/sportbladet/speltips/"], a[href*="aftonbladet.se/kampanj/"]
aftonbladet.se##:matches-path(/^/$/) p:has-text(Artikeln innehåller annonslänkar):upward(a)
aftonbladet.se##[data-ad-subtype]:upward(1):matches-css(min-height:/[0-9]+/)
aftonbladet.se,godare.se,livsstil.se##div[data-test-tag="prisjakt-carousel"], a[href^="/brandstudio"], div[class^="advertory-"]:not(.advertory-header-anchor)
aftonbladet.se,godare.se,livsstil.se,skonhetsredaktorerna.se,omni.se,omniekonomi.se,svd.se##.sp-message-open body:style(overflow:initial!important; position:unset!important; margin-top:unset!important;)
aftonbladet.se,halsasverige.se,mandarinmedia.se,nojesmagasinet.nu,stoppapressarna.se,langd.se,pressbladet.se,svenskpress.se,foretagsbladet.se,gestrikemagasinet.se,cfanytt.se,lasarnas.se,hembostad.nu,sportidrott.se,skolvarlden.se,computersweden.se,thatsup.se,arbetaren.se,sjofartstidningen.se##.advert
aftonbladet.se,livsstil.se,godare.se,byggahus.se,expressen.se,elle.se,femina.se,svenskdam.se,galamagasin.se,rodeo.net,familjeliv.se,vitaestilo.se##+js(href-sanitizer, a[href*="/t?a="], ?url)
aftonbladet.se,skonhetsredaktorerna.se##.ab_responsive_ads
agriaffaires.se,truckscorner.se,machineryzone.se##.dp--mb
aikfotboll.se,vaken.se,tidningen.djurskyddet.se##.banners
aikhockey.se,almtuna.com,bikkarlskoga.se,bjorkloven.com,brynas.se,difhockey.se,frolundahockey.com,farjestadbk.se,hockeyallsvenskan.se,hv71.se,ikoskarshamn.se,kalmarhockey.com,leksandsif.se,lhc.eu,luleahockey.se,malmoredhawks.com,modohockey.se,moraik.se,nybrovikings.com,orebrohockey.se,roglebk.se,shl.se,skellefteaaik.se,sodertaljesk.se,taif.nu,timraik.se,vaxjolakers.se,vikhockey.se,vik.se,ostersundik.com##a[href*="svenskaspel.se"][target]
aip.nu##[class*="feed-ad"]
aip.nu,funktionshinderpolitik.se,sjostadsbladet.se,fotbollsresultat.com,lansposten.se,dalabygden.se,sormlandsbygden.se,skaneplus.se###cookie-notice
aip.nu,lansposten.se,dalabygden.se,sormlandsbygden.se##body.cookies-not-set:style(overflow:unset!important)
akaviaaspekt.se##.article-list-item--native, a.article-topic__list-item[href^="/annons"]
aktieskolan.se##section.elementor-section:has-text(Huvudsponsorer & partners)
aktiespararna.se,alekuriren.se,tidningen.se,kurera.se,vinbanken.se##.native
aktuellhallbarhet.se,byggindustrin.se,dagensmedia.se,dagensmedicin.se,fastighetsnytt.se,resume.se,dagenssamhalle.se,market.se,dagligvarunytt.se,privataaffarer.se##article:matches-css(after, content:/Annonssamarbete/i)
aktuellhallbarhet.se,byggindustrin.se,dagensmedia.se,dagensmedicin.se,fastighetsnytt.se,resume.se,dagenssamhalle.se,market.se,dagligvarunytt.se,privataaffarer.se##a[href^="/annons/"], a[href^="/native/"], .slot-module, .slot-articlemodule
aktuellhallbarhet.se,byggindustrin.se,dagensmedia.se,dagensmedicin.se,fastighetsnytt.se,resume.se,dagenssamhalle.se,market.se,dagligvarunytt.se,privataaffarer.se##div[class^="css-"]:matches-css(content:/Annons/i):upward(article)
aktuellhallbarhet.se,byggindustrin.se,dagensmedia.se,dagensmedicin.se,fastighetsnytt.se,resume.se,dagenssamhalle.se,market.se,dagligvarunytt.se,privataaffarer.se##div[class^="css-"]:matches-css(min-height: /420px|400px|320px|312px/)
aktuellsakerhet.se##a[href*="reklamsamarbete"]:upward(.td_block_wrap)
aktuellsakerhet.se##.block-title:has-text(Reklamsamarbete):upward(.td_block_wrap)
aktuellsakerhet.se##.block-title:has-text(Reklamsamarbete):upward(.td_block_wrap) + rs-module-wrap:remove()
aktuellsakerhet.se##.front-slider-reklamsamarbete, .category-gastkronika-reklamsamarbete, .front-top-reklamsamarbete
aktuellsakerhet.se##.td-adspot-title-span:upward(1)
aktuellsakerhet.se,borattforum.se,sjostadsbladet.se##.td-a-rec
alandstidningen.ax##.revive-wrapper, div[id^="block-views-block-editorial-ads"], div[id^="block-blockbanner"]
alekuriren.se##div[id^="aleku-"], #carouselVideoAd, #carouselVideoAdMobile, .native-bg, .casino
aletorget.se,alingsastorget.se,almhulttorget.se,alvestatorget.se,amaltorget.se,angelholmtorget.se,arbogatorget.se,arvikatorget.se,askersundtorget.se,askersundtorget.se,avestatorget.se,bastadtorget.se,bengtsforstorget.se,bjuvtorget.se,bodentorget.se,bollebygdtorget.se,bollnastorget.se,borastorget.se,borlangetorget.se,botkyrkatorget.se,bromollatorget.se,eksjotorget.se,enkopingtorget.se,eskilstunatorget.se,eslovtorget.se,fagerstatorget.se,falkenbergtorget.se,falkopingtorget.se,faluntorget.se,filipstadtorget.se,flentorget.se,forshagatorget.se,gallivaretorget.se,gavletorget.se,gislavedstorget.se,goteborgtorget.se,gotenetorget.se,gotlandtorget.se,hagforstorget.se,hallsbergtorget.se,hallsbergtorget.se,hallstahammartorget.se,halmstadtorget.se,haningetorget.se,harnosandtorget.se,harrydatorget.se,hassleholmtorget.se,hebytorget.se,hedemoratorget.se,helsingborgtorget.se,herrljungatorget.se,hoforstorget.se,hoganastorget.se,hoortorget.se,horbytorget.se,huddingetorget.se,hudiksvalltorget.se,hultsfredtorget.se,hyltetorget.se,jonkopingtorget.se,kalixtorget.se,kalmartorget.se,karlshamntorget.se,karlskogatorget.se,karlskogatorget.se,karlskronatorget.se,karlstadtorget.se,katrineholmtorget.se,kavlingetorget.se,kiltorget.se,kirunatorget.se,klippantorget.se,kopingtorget.se,kramforstorget.se,kristianstadtorget.se,kristinehamntorget.se,krokomtorget.se,kumlatorget.se,kungalvtorget.se,kungsbackatorget.se,laholmtorget.se,landskronatorget.se,leksandtorget.se,lidkopingtorget.se,ljungbytorget.se,ljusdaltorget.se,ludvikatorget.se,luleatorget.se,lundtorget.se,lyckseletorget.se,lysekiltorget.se,malmotorget.se,mariestadstorget.se,markarydtorget.se,marktorget.se,moratorget.se,nackatorget.se,nassjotorget.se,norrtaljetorget.se,nybrotorget.se,nykopingtorget.se,nynashamntorget.se,olandtorget.se,olofstromtorget.se,orebrotorget.se,orebrotorget.se,ornskoldsvikstorget.se,orusttorget.se,osbytorget.se,oskarshamntorget.se,ostersundtorget.se,osthammartorget.se,partilletorget.se,piteatorget.se,ronnebytorget.se,saffletorget.se,salatorget.se,sandvikentorget.se,sigtunatorget.se,simrishamntorget.se,sjobotorget.se,skaratorget.se,skellefteatorget.se,skovdetorget.se,skuruptorget.se,soderhamntorget.se,sodertaljetorget.se,sollefteatorget.se,sollentunatorget.se,solnatorget.se,solvesborgtorget.se,staffanstorptorget.se,stenungsundtorget.se,stockholmtorget.se,strangnastorget.se,stromstadtorget.se,sundsvalltorget.se,sunnetorget.se,svenljungatorget.se,tabytorget.se,tanumtorget.se,tidaholmtorget.se,tierptorget.se,timratorget.se,tingsrydtorget.se,tjorntorget.se,tomelillatorget.se,torsbytorget.se,tranastorget.se,tranemotorget.se,trelleborgtorget.se,trollhattantorget.se,trosatorget.se,uddevallatorget.se,ulricehamntorget.se,umeatorget.se,uppsalatorget.se,vallentunatorget.se,vanersborgtorget.se,varatorget.se,varbergtorget.se,varnamotorget.se,vasterastorget.se,vasterviktorget.se,vaxjotorget.se,vellingetorget.se,vetlandatorget.se,vimmerbytorget.se,ystadtorget.se##.collapse.row.jobb.annonslista,#sponsored,#banners-right,.mittenbanner,#banners-top,#banners-bottom
alexandrabylund.se,helahisingen.se,sportsnews.se,xn--sporthnt-5za.se###af-preloader
alghundklubben.com#@#.category-annons:not(body):not(html)
alkompis.se##app-ads, .cdk-overlay-container
alkompis.se##.cdk-global-scrollblock:style(overflow-y: initial !important; position: unset !important;)
allaaktier.se##div[id^="ad-"]
allabolag.se##article:has(.advert__mark)
allabolag.se###company-card_top-banner, .lwad
allabolag.se##.strossle-widget:upward(div[style^="min-height"])
allas.se,elle.se,femina.se,hant.se,mabra.com,residencemagazine.se,svenskdam.se,motherhood.se##article.grid:has(a[href="/creative-studio"])
allas.se,elle.se,femina.se,hant.se,mabra.com,residencemagazine.se,svenskdam.se,motherhood.se##article.grid:has-text(/annonssamarbete/i)
allas.se,elle.se,femina.se,hant.se,mabra.com,residencemagazine.se,svenskdam.se,motherhood.se##article[data-type="native"], .ag-product-wrapper, .product-carousel__container, .shop_carousel, .editorsPick, div[class^="strossle-widget-"], .ad-min-height, a.cts-impression-item[data-cts-label*="banner"], section[data-cts-label="affiliate-carousel"]
allas.se,elle.se,femina.se,hant.se,mabra.com,residencemagazine.se,svenskdam.se,motherhood.se##a.js_commercial-text--link-text:upward(.jwplayer_video-videoArea):remove()
allas.se,elle.se,femina.se,hant.se,mabra.com,residencemagazine.se,svenskdam.se,motherhood.se##a:has([data-type="Sponsored"])
allas.se,elle.se,femina.se,hant.se,mabra.com,residencemagazine.se,svenskdam.se,motherhood.se##div.wings-gray-200:has-text(Annons)
allas.se,elle.se,femina.se,hant.se,mabra.com,residencemagazine.se,svenskdam.se,motherhood.se##p:has-text(ANNONS:)
allas.se,elle.se,femina.se,hant.se,mabra.com,residencemagazine.se,svenskdam.se,motherhood.se##+js(aeld, blur, i.focusPlayerElement)
allas.se,elle.se,femina.se,hant.se,mabra.com,residencemagazine.se,svenskdam.se,motherhood.se##+js(aeld, scroll, t.view.updateBounds)
allas.se,elle.se,femina.se,hant.se,mabra.com,residencemagazine.se,svenskdam.se,motherhood.se##+js(href-sanitizer, a[href*=".io/c/"], ?u)
allatvkanaler.se##.gda, .cookie-notification
allsvenskan.se##a[href*="track.adform"]
alltforforaldrar.se###partnerMenuContainer, #partnerMenuContainerFiller
alltforforaldrar.se##.spons-artc, a[href^="/native/"]
alltforforaldrar.se##.unslider-wrap.unslider-carousel>li:has(.preamble-category:has-text(/^annons/i))
alltforforaldrar.se,di.se,upphandling24.se,bytbil.com,sverigesnatur.org,tv24.se,nyan.ax##.panorama
alltomarbetsmiljo.se##main > div:not([id]):not([class]):has(a[href$="nyhetsbrevet"])
alltomarbetsmiljo.se##.bg-native
alltomburgare.se##.newscolumn:has(a[href$="/sponsrat/"])
alltomelbil.se###zox-lead-top-wrap
alltomelbil.se##:is(.p-list, div[class*="post-"]):has(a[href*="/annons"])
alltomhif.se##a:has-text(/betting|utan registrering|casino/i):upward(article, .slide-item):remove()
alltomhif.se##.sek-module-inner a[target="_blank"]
alltomkungligt.se###banner-holder
alltomnorrtalje.se##.allto-widget, .allto-before-content, .allto-after-content, article[class*="sponsrad"]
alltomsallskapsspel.se##.bannersRight
alpresor.se###toast-container
altinget.se##a[href^="/sponsrade"]
antagning.se,universityadmissions.se###cookiebanner
arbetaren.se##.text-sm:has-text(/annons/i):upward(.border-b, a[target])
arbetet.se,tidningenelektrikern.se,fastighetsfolket.se,handelsnytt.se,ka.se,sekotidningen.se##.Container:not(.ContentItem-content):has([data-controller="ad"])
arbetet.se,tidningenelektrikern.se,fastighetsfolket.se,handelsnytt.se,ka.se,sekotidningen.se##.Teaser--native, .o-native, [data-controller="ad"], div[id^="consent-"]
arjeplognytt.se##.metaslider
arjeplognytt.se##p:has-text(ANNONS):upward(.et_pb_text)
arkitekten.se##div[id^="consent-"]
arkitekten.se##html:style(--scrollbar-width:initial!important)
arkitekten.se##.MediaWrapper-content:style(opacity:unset!important)
arkitektur.se##article:has(.Entry-sponsored)
arkitektur.se##[class*="panorama"]
artbannersplus&task=show
assistanskoll.se###annons
atl.nu,landlantbruk.se,land.se##a[href*="/atl-tv-annons/"], [class^="Ad_"], div[class^="WidgetCTASticky"]
atl.nu,landlantbruk.se,land.se#@#.ad-unit:not(.text-ad):not(.textads)
atl.nu,landlantbruk.se,land.se,di.se,expressen.se,dn.se###didomi-host
aurumforum.se##span:has-text(Annons):upward(2)
autolife.se###Banners
automation.se,verkstadstidningen.se,transportnytt.se,datormagazin.se##.a-wrap
autonytt.se###main > .col-links
autonytt.se##.label:has-text(/sponsrad/i):upward(a)
autonytt.se##.sidebar_content:has(a[href*="casino"])
autonytt.se,sv.picmix.com,tekniknytt.se##.leaderboard
autopower.se##.card:has(.adsbygoogle)
avanza.se#@#a[title="LeoVegas"]
aventyrsresor.se,travelnews.se##.newsletter-popup
babyhjalp.se##.elementor-widget[data-settings*="sticky_"], div[id^="babyhjalp_panorama"], div[id^="babyhjalp_mobil"], div[id^="stagi"]
bakasockerfritt.se###cookiescript_injected_wrapper
bandyfeber.com##article:has(a[href*="/annons-"])
bandyfeber.com##.slide-entry-excerpt:has-text(/annons:/i):upward(.avia-content-slider)
bandyfeber.com##.widget_sp_image, a[title^="ANNONS"], .inner_sidebar .widget_text, .entry-content a[href*="utm_campaign"]
banners$image,domain=travsport.se|gavletravet.se
baraenkakatill.se##.post-item__tag:has-text(/spons/i):upward(li.post-item)
barnistan.se,welma.se##.newsletter, a[onclick*="adClick"]
barnistan.se,welma.se,ingenjorsjobb.se##.cookie-notice
barnsemester.se##.puffLine, .d-flex > div[style*="min-height"], div[style="overflow-x: hidden;background-color:rgb(250,250,250);width:320px;min-height:200px;"], div[style="overflow-x: hidden;background-color:rgb(250,250,250);width:320px;min-height:320px;"]
barometern.se,blt.se,bt.se,kristianstadsbladet.se,olandsbladet.se,smp.se,sydostran.se,trelleborgsallehanda.se,ut.se,ystadsallehanda.se,vxonews.se,vaxjobladet.se,nsk.se,klt.nu##div:has-text(/^Annons/):upward(a)
barometern.se,blt.se,bt.se,kristianstadsbladet.se,olandsbladet.se,smp.se,sydostran.se,trelleborgsallehanda.se,ut.se,ystadsallehanda.se,vxonews.se,vaxjobladet.se,nsk.se,klt.nu##div[class*="AdWrapper"]:upward(1)
barometern.se,blt.se,bt.se,kristianstadsbladet.se,olandsbladet.se,smp.se,sydostran.se,trelleborgsallehanda.se,ut.se,ystadsallehanda.se,vxonews.se,vaxjobladet.se,nsk.se,klt.nu##div[class*="fluffy-Overlay"]:has(img[src*="-ad/"], img[src*="Checkout"])
barometern.se,blt.se,bt.se,kristianstadsbladet.se,olandsbladet.se,smp.se,sydostran.se,trelleborgsallehanda.se,ut.se,ystadsallehanda.se,vxonews.se,vaxjobladet.se,nsk.se,klt.nu###root > div:first-child:matches-css(position: fixed)
barometern.se,blt.se,bt.se,kristianstadsbladet.se,olandsbladet.se,smp.se,sydostran.se,trelleborgsallehanda.se,ut.se,ystadsallehanda.se,vxonews.se,vaxjobladet.se,nsk.se,klt.nu##.component_guide-ads, #fullpage-ad-portal, div[style="min-height: 302px;"]
barometern.se,blt.se,bt.se,kristianstadsbladet.se,olandsbladet.se,smp.se,sydostran.se,trelleborgsallehanda.se,ut.se,ystadsallehanda.se,vxonews.se,vaxjobladet.se,nsk.se,klt.nu##:is([id*="_panorama"],[id*="_mobil"]):upward(div[display="block"])
barometern.se,blt.se,bt.se,kristianstadsbladet.se,olandsbladet.se,smp.se,sydostran.se,trelleborgsallehanda.se,ut.se,ystadsallehanda.se,vxonews.se,vaxjobladet.se,nsk.se,klt.nu##:is([id*="_panorama"],[id*="_outsider"],[id*="_insider"],[id*="_mobil"]):upward(1)
battregolf.se##article.elementor-post:has(a[href*="casino"], a[href*="bonus"], a[href*="betting"], a[href*="/noje/"])
battregolf.se##.elementor-element[data-widget_type="image.default"]
battrestadsdel.se###top-banner-mobile, .apd-text, .apds_main, .entry-priomaker, [class^="dls-"], .csmi
battrestadsdel.se,flashback.se,leta.se###top-banner
beernews.se##.cookie-consent-wrapper, #takeover-outer
bergsmannen.se,tidningenbyggmaterial.se##.ann-puff, .headerLinks
besoksliv.se##a[href*="sponsrat-innehall"], div[class$="-promotion"]
bestchampagne.se##aside.section-sm
bettips.se##.bettips-am
bettips.se,borskollen.se,se.azrhymes.com##.top-banner
biblioteksforeningen.se##body:style(opacity:1!important)
biblioteksforeningen.se,psykologiguiden.se,rabattsok.se###cookie-bar
bike.se##.post-block-style:has(a[href*="/annons"])
bildobubbla.se##.annonser
bilresaieuropa.se###header-image, #block-2
bilresaieuropa.se##.widget-title:has-text(/spons/i):upward(.widget_text)
bilsport.se##fl-gdpr, fl-panorama-top, fl-newsletter-popup
bilsport.se##.includingFeaturedSliderArticle:has(.native-mark)
bilwebben.ax##.front #secondary-content-wrapper, .banner-wrapper, .content-prefix-banner-wrapper
bioenergitidningen.se##article:remove-class(closed)
bioenergitidningen.se###cookieinfo
biostock.se,hejauppsala.com,svenskfilmdatabas.se,bredband.se##.wt-cli-cookie-bar-container
biostock.se,tobaksfakta.se##.pum-open:style(overflow:auto!important)
birthday.se##.datax
bjuvsweek.se##.carouselbanner-wrp
blocket.se##.placement_panorama, .blocket-placement, div[style="height: 240px;"], [class*="offering-info-box"], [data-id="placement_panorama"], div[class*="BannerLink"]
bohuslaningen.se,stromstadstidning.se,markposten.se,harrydaposten.se,partilletidning.se,sttidningen.se,molndalsposten.se,kungalvsposten.se,kungsbackaposten.se,alingsastidning.se,ttela.se,gp.se,hallandsposten.se,hn.se,mellerudsnyheter.se##.c-ad__panorama, .c-ad__insider, #outsiderTop, div[data-k5a-pos^="panorama"]
bokadirekt.se##a:not([href*="bokadirekt.se"]):not([href^="/"]) img
bokadirekt.se##.ReactModalPortal:has(a[href="/articles/cookies"])
bokmassan.se,svenskamassan.se##.cookie-law
boktugg.se##.elementor-section:has(.sponsor, .elementor-post.category-sponsrat)
boktugg.se##[id^="boktu-"]
boneo.se##.article-top-advt
boneo.se##.slick-slide:has-text(/sponsra/i)
booli.se###outer
borattforum.se##.meta-info-container:has(a[title*="Sponsrad artikel"])
borskollen.se##a:has(.sponsored)
borskollen.se##img[src*="/borskollen_newsletter"]:upward(1)
borskollen.se##.adlabel:upward(1)
borskollen.se##.colorized:has-text(/annons/i):upward(a)
borskollen.se##.elevated-button:has-text(/^Cookie/):upward(.container)
borskollen.se##.label:has-text(/annons/i):upward(1)
borskollen.se##.main > div[class^="jsx-"]:last-of-type:has(img[src*="borskollen_appen"])
borskollen.se##.outer:has(img[src$="ad_label.png"])
borskollen.se##.sponsored-chip:matches-css(display: block):upward(a)
borskollen.se##.wrapper > div[class^="jsx-"] > .outer:has(a[href*="casino"])
borskollen.se##[id^="borskollen_small"], [id^="borskollen_large"], .featured-link, .app-store-box, #borskollen_desktop-side, #borskollen_desktop-panorama, div[id^="borskollen_mobile-detaljsida"]
borssnack.di.se##.bn_advertisement__panorama, .bn_advertisement__container
borsvarlden.com##article:has(.border-sponsored)
borsvarlden.com##.label:has-text(/annons/i):upward(.highlighted-article-block)
borsvarlden.com##.sponsored-articles-container, .nav-sep-blink, .annons-label, .index-side-banner-wrapper, .index-top-banners-wrapper, .fullwidthbanner-container, .banner-wrapper
bovision.se##a:has(.ad-mark)
bovision.se##.banner-image
bovision.se##.blog-article-card:has(.sponsor-mark)
brafiler.se###header-banner, #cboxOverlay, #colorbox, .adv-inner, #sidebar-banner
brafiler.se##.rlt-top-pro:has(a[href*="casino"])
branschaktuellt.se##span:has-text(Sponsrad):upward(.article)
branschaktuellt.se##.popup-signup, .takeover
branschkoll.se##div[id^="brans-"], .widget-sponsored-post
branschstegen.se##.container:has(a[href*="casino"])
branschstegen.se##[class*="sponsored"], #watcherPop, .modal-backdrop
breakit.se##section[class*="Article_layout"]:has(section[class*="Sponsored"])
breakit.se##[class*="sponsored"], [class*="Sponsored"], [class*="LivepodPuff"], .videoAd, .js-video-ad, [class*="AdkContainer"], div[class^="LivewrappedContainer_root"]
brollopstorget.se##.bt-article:has(a[href*="/annons/"])
bukefalos.se,thaisnack.se,rollspel.nu,husbilsklubben.se,friaordet.org,xn--lnforum-exa.se,ihusbil.se##.u-bottomFixer
bulletin.nu##div[class*="section-preview"]:has-text(/betalt samarbete/i):upward(4)
bulletin.nu##[class^="newsletter-subscribe"], div[class^="cookie-message"], div[role="presentation"]
bulletin.nu,inredningsarkitektur.se,fof.se,allas.se,elle.se,femina.se,hant.se,mabra.com,residencemagazine.se,svenskdam.se,motherhood.se,aftonbladet.se,lchfarkivet.se,kollega.se,folkofolk.se,skyscanner.se,dagensarena.se,bokadirekt.se,barometern.se,blt.se,bt.se,kristianstadsbladet.se,olandsbladet.se,smp.se,sydostran.se,trelleborgsallehanda.se,ut.se,ystadsallehanda.se,vxonews.se,vaxjobladet.se,nsk.se,klt.nu,samnytt.se,sjofartstidningen.se##body:style(overflow:initial!important)
bussmagasinet.se###page > div:not(.left):not(.right)
bussmagasinet.se###titlebanner
bussmagasinet.se,byggteknikforlaget.se,dialasen.com,torbjornstips.se,backpacking.se,kanadaresa.se,usa.se,sporthalsa.se,ravarumarknaden.se,livetsgoda.se,opulens.se,radiotreby.se,nyadagbladet.se,fiskemagasinet.se,etunanytt.se##.textwidget a[target="_blank"]
butikstrender.se##a[target="_blank"] picture, div[data-settings*="sticky"], div[id^="butik-"]
butikstrender.se##body > .elementor > .elementor-section:first-child:has-text(Annons)
byggahus.se##a.click-track, img.click-track:remove-class(click-track)
byggahus.se##a.click-track-attachment-preview, img.click-track-attachment-preview:remove-class(click-track-attachment-preview)
byggahus.se##body.forum-logged-out .svartalistan-results-login-required:style(height: unset !important;)
byggahus.se##img[data-click-track]:remove-attr(data-click-track)
byggahus.se##+js(aeld, /adblockDetector|adsInserted|partnerExternalLinkClick/)
byggahus.se##.bbImageWrapper--preview.active img:style(-webkit-filter:none!important; filter:none!important; transform:none!important; -webkit-transform:none!important;)
byggahus.se##.block-ad, #cookie-consent-dialog, a[href^="/partner/"], .threadMatchedContent, #svartalistan-login-required-overlay
byggahus.se,expressen.se,filmtopp.se,destination.se,spokbloggen.nu,folkhalsasverige.se,foretagsverige.se,forskningsverige.se,motorbibeln.se,hallbarhetsverige.se,tillvaxtsverige.se,grillbibeln.se,kampenmotcancer.se,bolagsfakta.se,affarsvarlden.se,affarerinorr.se,viivilla.se##.ad-container
byggfaktadocu.se##.pop_box
byggfakta.today,citymark.today,hotellorestaurang.se##.cookie_popup_box
byggipedia.se##aside .textwidget:has-text(/sponsr|samarbetspartners/i)
byggipedia.se##*:style(user-select: auto !important;)
byggipedia.se##+js(acs, document.onkeydown, e)
byggipedia.se##+js(acs, document.onkeypress)
byggipedia.se##+js(acs, frames, oncontextmenu)
byggipedia.se##+js(acs, jQuery, contextmenu)
byggipedia.se##+js(set, ai_set_cookie, noopFunc)
byggipedia.se##.code-block:has(.adsbygoogle)
byggipedia.se##.protect_contents-overlay, .ai_widget
byggkontakt.nu##a:has-text(/poker|casino|kasino|betting/i):upward(li)
byggnadsarbetaren.se##[class^="siteAds"], .siteAlerts, #gan-popup
byggteknikforlaget.se###text-2.widget_text, .header-widget-area
byggvarlden.se,omtanke.today##a[href*="/annons/"], .newsletter-popup-content-overlay, .newsletter-popup, .ai-viewports
byggvarlden.se,omtanke.today##.post:has(a[href*="/annons/"])
bytbil.com##html,body:style(overflow: auto !important;)
bytbil.com###privacyModal
bytbil.com##.available-services
cafe.se,kingmagazine.se##.card-partner:upward(1)
cafe.se,kingmagazine.se,mestmotor.se##.card-partner, .partner
campingsverige.se##.banner_window, .banner_label, .card_veckans_pryl, .bg_camping_se
campingsverige.se##.post_sponsrad_label:upward(1)
camping.se##.ads-above-header, .ads-teaser, .paragraph--type--ad-script, div[about*="/annons/"], a[href*="/sv/annons"]
canariajournalen.se##.highlighted:has(.advertisement)
cannabisifokus.se##div[id^="canna-"]
cannabis.se##+js(aopw, Cookies)
cannabis.se##.header-ads-wrapper, .ai-adb-hide, .ai-sticky-widget, .hampaonline
cannabis.se,biostock.se,snowmobile.se,tobaksfakta.se,dagenslogistik.se,magasinetkonkret.se,skaneplus.se,battrestadsdel.se##.pum-overlay
carup.se##div[id^="carup-"]
casinoguiden$image,domain=samnytt.se|samnytt.nu
casino$domain=pirkt.se
casino-utan-$image
cfosvepet.se##.recent-post-item:has(a[href="#"]:not(.w-condition-invisible))
chefstidningen.se##[id^="block-views-ad"], .modal-container
chef.se##.Cookie-notice, .Product-modal, .Offer-popup, .Toaster
chef.se,fokus.se##.Blurb--native
cineasten.se###text-6, .theiaStickySidebar .category-uncategorized
cineasten.se##.ajax_loader
computersweden.se##.nativo
computersweden.se##.latest-content__card-secondary:has(.nativo)
com.se,~www.com.se##html::before:style(content: "OBS! VARNING! Om denna sida är en butik så är det förmodligen en bluffbutik. Detta är ett meddelande från det svenska filtret i din annonsblockerare." !important; font-size: 18px !important; font-family: sans !important; background-color: red !important; color: white !important; padding: 6px !important; width: 100% !important; display: block !important; text-align: center !important;)
conpot.se##div:has-text(ANNONS):upward(article:not([id]))
conpot.se##+js(set, square_array1, null)
conpot.se##+js(set, square_arraytop, null)
cookaholic.se###loftloader-wrapper
cookie-consent$domain=upphandling24.se
cornucopia.se###sponsrade-lankar:upward(aside) + aside.widget_block
corren.se,folkbladet.se,mvt.se,nt.se,vt.se,vimmerbytidning.se,kuriren.nu,nsd.se,norran.se,pt.se,ekuriren.se,strengnastidning.se,kkuriren.se,sn.se,eposten.se,unt.se,helagotland.se,kindaposten.se,gotlandjustnu.se##ad-iris-sunt-ad-wrapper, ad-block, .native, ad-full-page-block, a[href^="/native"], widget-family, widget-memorial, widget-marknadsguiden, widget-jobb-plus, a.puff-primary-link[href*="/erbjudande/"], .ad-hidden, iris-puff-native
corren.se,folkbladet.se,mvt.se,nt.se,vt.se,vimmerbytidning.se,kuriren.nu,nsd.se,norran.se,pt.se,ekuriren.se,strengnastidning.se,kkuriren.se,sn.se,eposten.se,unt.se,helagotland.se,kindaposten.se,gotlandjustnu.se##iris-subscribe-footer
corren.se,folkbladet.se,mvt.se,nt.se,vt.se,vimmerbytidning.se,kuriren.nu,nsd.se,norran.se,pt.se,ekuriren.se,strengnastidning.se,kkuriren.se,sn.se,eposten.se,unt.se,helagotland.se,kindaposten.se,gotlandjustnu.se,tv.nu,klart.se##.sp-message-open body:style(overflow:unset!important;position:unset!important;)
curateContext=affiliate$domain=aftonbladet.se
cykelframjandet.se##:is(article.tg-item, .lcp_catlist li):has(a[href*="/annons"])
cykla.se##.featured-post--sponsored, .grid-item--sponsored, #advert-once-banner-fullskarm
cykla.se#@#.advertisment
dagensarena.se##.popup
dagensinfrastruktur.se,nyaprojekt.se,nordiskaprojekt.se,svenskbyggtidning.se,grontsamhallsbyggande.se##.g-single, a[onclick*="banner"], a[onclick*="advert"], .adrotate
dagensjuridik.se##strong:has-text(/^senaste nytt från våra partners/i):upward(.card--muted)
dagensjuridik.se##.outher-sidebar, a[href*="/annons/"], .dj-inline-ad
dagenslogistik.se##div.g, .top-banner
dagenslogistik.se##small:has-text(/annons/i):upward(.elementor-column)
dagensps.se##a[href*="/ps-partner"]:upward(section.cat-post-widget)
dagensps.se##a[href*="/ps-partner/"], .ad-links-module, .dagensps_ad, a[href*="ut.dagensps.se"][target], .bottom_banner, .leftsidebanner, .c-external-notice
dagensps.se##div[class^="bg-"]:has(a[href="/ps-partner"])
dagensps.se##.container:has(.dagensps_ad)
dagensps.se##.postbox:has(.sponsored_post)
dagensps.se##:is(.text-text-secondary, span.font-bold):has-text(ANNONS):upward(2)
dagenstech.se##a[href^="https://dagenstech.se/articles/"]:upward(1):has-text(SPONSRAT)
dagenstech.se##.banner-desk, .banner-mob
dagenstech.se##.text-right:has-text(ANNONS)
dagenstv.com##.slick-slide:has-text(/casino/i)
dagenstv.com,kolla.tv##.grid-add-container
dagensvimmerby.se,dagensvastervik.se,dagenskalmar.nu,dagenshultsfred.se##body:style(margin-top: 0 !important;)
dagensvimmerby.se,dagensvastervik.se,dagenskalmar.nu,dagenshultsfred.se##.panoramaAnnons, .JobAdDiv, .annonsKolumn, .insideAd, .ingressAd, .familyAds, .annonsWrapper
dagens.se##.item:has(.prebid, div[data-ad-unit-id], a[href*="casino"])
dagen.se##.video-annons, .native-box, .arcad-block-container
danskaspraket.se##.rightcol
darkside.se##a[href*="?aktion=bannerclick"]
datormagazin.se##a:has-text(/^annons/i)
datormagazin.se##div[id^="dator-"]
datormagazin.se##.heading:has-text(/samarbete/i):upward(.elementor-widget-smartmag-featgrid)
datormagazin.se##.td-big-grid-post:has(a[href*="/samarbete/"])
datormagazin.se##.td_module_wrap:has(a[href*="/annons/"])
dayviews.com##.frontPageBox--links
da.se##.Advert
deliquate.se##[id^="ads300"], [id^="linkcat-"]
densistavilan.se##div[data-advadstrackid]:upward(.x-bar-footer)
densistavilan.se##h3:has-text(Advertorial):upward(1)
densistavilan.se###fancybox-wrap, div[id^="densi-"]
dental24.se##.fp_banners, .cypress-popup_newsletter
dental24.se##.post-box:has(.sponsored)
designbase.se##html,body:style(overflow:unset!important;)
designbase.se##.banner-hidden, .z-newsletter-modal, .z-newsletter-popup
desktop-banner$image,domain=bokadirekt.se
destination.se,sistaminuten.se##+js(set-cookie, CM_cookieConsent, 0)
devote.se##article.tile:has-text(/annons|spel|casino|kasino/i)
devote.se##div[data-losjs^="borka"]:upward(1)
devote.se##+js(aeld, click)
devote.se##.slick-slider
devote.se,familjeliv.se##div[style*="height: 244px;"]
digitalavykort.se##.rightdiv p:has-text(/casino|kasino|lån|betting|odds|lotto/i)
digitalfotoforalla.se,iform.se,pctidningen.se,varldenshistoria.se##li:has(.content-label:has-text(/annons/i)):remove()
digitalfotoforalla.se,iform.se,pctidningen.se,varldenshistoria.se##.scroll-message, .gallery-banner, .horseshoe, [data-ad-type], .bcm-banner
digitalfotoforalla.se,iform.se,pctidningen.se,varldenshistoria.se##.teaser:has(.teaser__cat--sponsorlabel)
digitalfotoforalla.se,pctidningen.se##.opacity-fade:style(opacity:1!important; transition:none!important; animation:unset!important;)
dinamediciner.se##.top-header:has(.adsbygoogle)
dinbyggare.se##article.category-leverantorer, div[style^="\[banner-style\]"]
dinbyggare.se##p[style="text-align: center;"]:has(a[target] > img)
dinbyggare.se##*:style(-webkit-touch-callout: default !important; -webkit-user-select: text !important; -moz-user-select: text !important; -ms-user-select: text !important; user-select: text !important;)
dinbyggare.se##+js(rmnt, noscript)
dinbyggare.se##+js(rmnt, script, /wccp_pro/)
dinbyggare.se##::selection:style(background-color:#007aff!important;color:#fff!important;)
dinvinguide.se##.contain:has(a[target="_blank"])
discoveringtheplanet.com##body:remove-class(unselectable)
discoveringtheplanet.com##html:style(user-select:unset!important; -moz-user-select:unset!important; -webkit-user-select:unset!important;)
discoveringtheplanet.com##+js(acs, disableEnterKey)
discoveringtheplanet.com##+js(acs, document.ondragstart)
discoveringtheplanet.com##.widget-title:has-text(/annons/i) + .textwidget
di.se##+js(set, getAdblockerStatus, noopFunc)
di.se##.di_panorama-wrapper, .site-header__panorama, .di_panorama__isAdLabel, .discount-box, .campaign-ad-box, .di_start__teaser-placeholder, .di_teaser-flak-planbokskoll, .di_teaser-flak-container--native, .native-box, .bandit-box__teaser--native, a[href*="/brandstudio"], .service-box, .brand-studio-box, .native-article, .listing-box-native
di.se##.market-start-top + div:not(.market-container__wrapper)
djungeltrumman.se##strong:has-text(/samarbete|sponsrat/i):upward(li):remove()
djungeltrumman.se###sponsored-posts, #right-banners, .banner-wrapper, .top-banner-label, .banner-label
djungeltrumman.se##.label-sponsored:upward(#latest-slider a):remove()
djungeltrumman.se##.post:has(.label-sponsored)
dn.se##body:style(position:unset!important;overflow-y:scroll!important;)
dn.se##.article--native, .teaser-card--native, .ds-teaser--native, #dnse-popup
dn.se##.campaign-holder
dn.se,di.se##video:remove-attr(data-auto-play)
dn.se,di.se##.teaser-native
dn.se,di.se,expressen.se,atl.nu,landlantbruk.se,land.se,hd.se,sydsvenskan.se,allehanda.se,tidningenangermanland.se,arbetarbladet.se,avestatidning.com,bblat.se,dalademokraten.se,fagersta-posten.se,gd.se,lt.se,ltz.se,na.se,norrteljetidning.se,nynashamnsposten.se,op.se,salaallehanda.com,st.nu,tidningenharjedalen.se,vlt.se,falkopingstidning.se,jp.se,skaraborgslanstidning.se,skovdenyheter.se,smalandsdagblad.se,smalanningen.se,smt.se,tranastidning.se,vastgotabladet.se,vetlandaposten.se,vn.se,bandypuls.se,ljusdalsposten.se,ljusnan.se,soderhamnskuriren.se,ht.se,moratidning.se,borlangetidning.se,falukuriren.se,sodran.se,nyaludvikatidning.se,skd.se,nvp.se,nuiosteraker.se,netdoktorpro.se,popularhistoria.se,aktuellhallbarhet.se,byggindustrin.se,dagensmedia.se,dagensmedicin.se,fastighetsnytt.se,resume.se,dagenssamhalle.se,market.se,dagligvarunytt.se,privataaffarer.se,barometern.se,blt.se,bt.se,kristianstadsbladet.se,olandsbladet.se,smp.se,sydostran.se,trelleborgsallehanda.se,ut.se,ystadsallehanda.se,vxonews.se,vaxjobladet.se,nsk.se,klt.nu,illvet.se,pctidningen.se,digitalfotoforalla.se,iform.se,varldenshistoria.se,slakthistoria.se##body.didomi-popup-open:style(overflow:unset!important)
doktorn.com##.js-banner-wrapper
doktorn.com##.js-cookie-disclaimer
doon.se##.doon-promotion, a.link[target="_blank"]
driva-eget.se##.sponsored_content
dust2.se##html[data-impression-tracking-endpoint]:remove-attr(data-impression-tracking-endpoint)
dust2.se##.main-page-content:style(background-image:none!important;)
dust2.se##.target-banner, div[data-type="BANNER"]
dykarna.nu###rightbanners
edgeflyfishing.com###g-header, #g-aside, #g-sidebar, div[data-role="sidebarAd"]
ehandelstips.se##:is(li, article):has([href*="/sponsradeartiklar/"])
ehandel.se##.aside-list--heading:has-text(/^sponsra/i):upward(.aside-list)
ehandel.se##.code-block:has-text(/annons/i)
ehandel.se##.commercial-row, .aside-image-with-link, .post-container-sponsored, aside a[href*="/branschnyheter/"]
ekonominyheter.se###lblock-ads
ekonominyheter.se##.td-fix-index:has(a[href*="casino"])
ekonominyheter.se,autonytt.se,undervarttak.se,aftonbladet.se,lesscarbs.se,hockeybladet.nu,matinspo.se##a[href*="/track.adtraction."]
electronic.se##.content aside.column-narrow:last-of-type
elektronikforumet.com##td > a[target="_blank"] img
elevspel.se##div#cookie_wrapper
elevspel.se##div[class*="-unit"]:has(a[href="/medlem/plusmedlem.html"])
elevspel.se##+js(rmnt, script, cloned.removeAttr)
elle.se##section.c-native_banner:upward(2)
emocore.se###main > #home_start_div ~ .m_t.box:nth-last-child(-n+2)
emocore.se###sticky-panorama-container, #mob-wrap
energi.se##.advertisement--item
eniro.se##article:has(#marketing)
eniro.se##div.rounded-4xl:has(a[href$="/firma#marketing"])
epochtimes.se##.fixed.bottom-0
esportare.se##a[href*="utm_campaign"]
esportare.se##em:has-text(Annonser):upward(2)
esportsacademy.se###preloader
espressomedia.se##div[id^="espre-"], .category-native
espressomedia.se##.penci-block-vc:has([href*="casino"])
etc.se##.adaptive:upward(1)
etc.se##.paywalled.hidden:style(display:unset!important)
etc.se##[data-controller="ad-container"], .bg-gradient-white
etn.se,uppsalanyheter.se,rotter.se##.banneritem
etunanytt.se##.textwidget:has-text(ANNONS)
etunawebben.se##+js(nostif, ad)
europaportalen.se##.view-multiply-top
eu-cookie$domain=skidspar.se
eventeffect.se###secondary > .widget:nth-child(2)
eventeffect.se,executiveeffect.se,saleseffect.se##.partnerartikel, #sidebar-ads-right, #nyhetsbrev-pp-wrapper__container
eventeffect.se,executiveeffect.se,saleseffect.se##.post-teaser:has(a[href$="/annons/"])
evergreengarden.se##article.elementor-grid-item:has-text(reklamsamarbete)
evertiq.se##+js(acs, $, banner_loader)
evertiq.se##.cc-container, [data-gabnr], #carpet
evertiq.se,fz.se##.bnr
everysport.com##div[id^="everysport_sky"], img[alt="X3000"], img[alt="Casinofeber"]
everysport.com##:is(div[id^="everysport_pano"], div[id^="everysport_rektangel"]):upward(1)
exakt24.se##section[data-ha-element-link*="kampanj"], .elementor-element-686a3aa6, .elementor-popup-modal
existenz.se##.link:has(a[href*="bannerid="])
existenz.se##.wm-nopop, #main > p[style^="color"], #slidebox
existenz.se,funfunfun.se,elektronikforumet.com##a[href*="bannerid"]
expo.se##div.flowy-wp-protected-content:remove-class(flowy-wp-protected-content)
expo.se##p.has-text-align-center:has-text(Annons:)
expo.se##.ad-image, .bottom-popup
expressen.se##.campaign
expressen.se##a:remove-attr(data-t-label)
expressen.se##a:remove-attr(data-t-type)
expressen.se##a[href*="/spel.exp"], a[href*="/lanapengar.exp"], a[href*="/rabattkoder.exp"], a[href*="/annons"], .match-betting, .discount-ad, .b-ad__caption, .pressrelease-teaser, .widget-ad-marker, .widget-ad-marker + a, .promotion-banner, .widget--collaboration, .rotator--external, a[data-click-track*="prisjakt"], .linked-image-widget a[href*="/kampanj/"], .linked-image-widget a[href*="lifestyle.expressen.se"], #premiumAdWrapper, .tapet-popup-overlay, .outsider-ads, .teaser > a[href*="/kampanj."], .teaser > a[href*="/brandstudio"], .teaser > a[href*="/brand-studio"], figure[data-article-data*="/sponsrat"], figure[data-article-data*="/annons"], figure[data-article-data*="/brand-studio"], .teaser--native, .native-article
expressen.se##strong:has-text(/^annons:/i):upward(p)
expressen.se##.html-widget > div[style^="text-align: center; font-size: 10px;"]
expressen.se##.tapet-popup-js-no-scroll, .tapet-no-scroll:style(overflow-y:initial!important; position:unset!important;)
expressen.se##.teaser:has(a[href*="/annons"], a[href*="/brandstudio"], a[href*="/brand-studio"], a[href*="/kampanj."], a[href*="/lanapengar."], a[href*="/rabattkoder."], a[href*="/spel.expressen.se"], .vignette--svg + a[href*="teknikensvarld."], .teaser__bottom--ad-marker)
expressen.se,di.se,nsk.se,skd.se,nvp.se,nuiosteraker.se,barometern.se,blt.se,bt.se,kristianstadsbladet.se,olandsbladet.se,smp.se,sydostran.se,trelleborgsallehanda.se,ut.se,ystadsallehanda.se,corren.se,folkbladet.se,mvt.se,nt.se,vt.se,klt.nu,vimmerbytidning.se,kuriren.nu,nsd.se,norran.se,pt.se,ekuriren.se,strengnastidning.se,kkuriren.se,sn.se,eposten.se,unt.se,helagotland.se,kindaposten.se,folkbladet.nu,vk.se,vasterbottningen.se,mellanbygden.nu,nordsverige.se,lokaltidningen.nu,vasterastidning.se,mitti.se,thelocal.se,byrum.se,sverigespringer.se,recept.se,viivilla.se,mestmotor.se,babyhjalp.se,fragbite.se,ibnytt.se,realtid.se,cafe.se,kingmagazine.se,vxonews.se,vaxjobladet.se,alekuriren.se,nyheter24.se,svenskgolf.se,golfing.se,gotlandjustnu.se,familjeliv.se,praktisktbatagande.se,norrahalland.se,lokalti.se,lchfarkivet.se,alltforforaldrar.se,idrottensaffarer.se,vf.se,hjotidning.se,kt.se,kt-kuriren.se,sla.se,mariestadstidningen.se,filipstadstidning.se,fryksdalsbygden.se,nwt.se,arvikanyheter.se,nkp.se,saffletidningen.se,provinstidningen.se,dalslanningen.se,nlt.se,skaraborgsbygden.se##+js(json-prune, autoplay)
extraextra.se##.sm-text:has(.adsbygoogle)
extrakt.se,macken.xyz,dialasen.com,lakartidningen.se,ordmedzcxy.se###cmplz-cookiebanner-container
familjehemsbanken.se,familjehemmet.se###cookieNotice
familjeliv.se##article:has-text(/annons:/i)
familjeliv.se##a[href*="/kampanj/"], .flm-kampanj
familjesidan.se##.cookies-wrapper
fastighetssverige.se##a[href*="/banner/out/"], .bnr_box, div[class^="panel"][style*="lightgoldenrodyellow"]
fastighetssverige.se##.featured-article:has(.badge-partner-text)
fastighetstidningen.se##.adspace, a[class*="annons"]
fasting.nu##body:style(display:unset!important)
feber.se,tjock.se##f-internallinks-new:has-text(Annons)
feber.se,tjock.se##+js(nosiif, checkGDPRInt)
feber.se,tjock.se##+js(set, dovideostuffAD, noopFunc)
feber.se,tjock.se##.burt-unit, .art_ad, adline, f-panorama, f-deals, #rpPopular, #maxetiseFull, #outsider, [data-ad="true"]
festivalinfo.se##a[title*="Casino"], #top-content
festivalinfo.se##.node-news:has(a[href*="casino"])
fightermag.se##article:has(a[href*="betting"], a[href*="casino"], a[href*="kasino"], a[href*="/gastskribent/"])
fightermag.se##a[href*="/sponsra"], #partners
filatelisten.se##:is(a[target="_blank"]:not([href^="/"], [href*="filatelisten.se"])):upward(section)
filmparadiset.se##.jnews-cookie-law-policy, a[href*="casino"], .custom-html-widget a[target="_blank"]
filmtipset.se##em:has-text(/sponsrad/i):upward(.row.news)
filmtipset.se###topslider-wrapper + .container > .sidebar, .sidebar a[target="_blank"], .sidebar a[href*="casino"], .sidebar a[href*="betting"], .sidebar a[href*="automater"]
filmtipset.se##.news:has-text(casino)
filmtipset.se##.row.news > div[style^="border"]:last-of-type
filmtopp.se##body:style(overflow:initial!important)
filmtopp.se##.cooperation-banner__container, .takeover-desktop, .takeover-mobile, #discover-banner
finanstid.se##.tdm-descr:has-text(/casino/i)
findit.se##+js(set, testPrebid, noopFunc)
findit.se##.banner-wrapper, .col-banner
firstclassmagazine.se###leader-wrap, #rpwe_widget-2
firstclassmagazine.se##.feat-cat:has-text(/annons/i):upward(a)
firstfoto.se##article.status-publish:has-text(/annonssamarbete/i)
firstfoto.se###cookie-consent-banner
fisheco.se###page-section-2, #page-section-24, .add-special-banner, .g-single
flamman.se##.Banner, .TakeOverBanner, .CookieNotice, div#popup
flashback.org###top-banner-container, #top-banner-wrapper
flashback.org##+js(nostif, #top-banner-container)
flashscore.se##.boxOverContent--a, .otPlaceholder, .seoAdWrapper, .adsbackground-wrapper, .prematchOddsBonus__bonus, .prematchLink[target], .detailLeaderboardSkeleton
flm.nu##.spons
flygtorget.se###PreHeader
fl-net.se##a:has-text(/lån|casino|kasino/i):upward(p)
fl-net.se###spopup
fl-net.se##.thumbnail:has([data-revive-zoneid])
fn.se###cookie
fodertipset.se##.fodertipset-org-banner
fof.se###CybotCookiebotDialog, #CybotCookiebotDialogBodyUnderlay
fof.se##.mediaconnect-protected-content .Carousel:style(opacity:unset!important;)
fof.se,elinstallatoren.se,spraktidningen.se,modernpsykologi.se,vvsforum.se##.mediaconnect-protected-content, .mediaconnect-protected-content--show:style(max-height: unset !important; overflow: unset !important;)
fof.se,elinstallatoren.se,spraktidningen.se,modernpsykologi.se,vvsforum.se##.mediaconnect-protected-content::after:style(background: unset !important;)
fokus.se##.sesamy-protected-content.active::after:style(background:unset!important;)
fokus.se##.sesamy-protected-content:style(max-height:unset!important;overflow:unset!important;)
folkofolk.se##div[class^="MuiDialog-root"]
foodfolder.se###myModal, .adImage
foretagande.se##article:has(.sponsored-text)
foretagande.se##div.article:has(a[href$="artiklar-i-samarbete"])
foretagande.se##div[id*="panorama"], .panorama-pos
foretagsverige.se,forskningsverige.se,motorbibeln.se,hallbarhetsverige.se,tillvaxtsverige.se,grillbibeln.se,kampenmotcancer.se,folkhalsasverige.se##:is(div[class*="vicky-whitebox"], .vicky-category-label, .vicky-video-infobox-label, .vicky-post-headline-container__category__inner):has-text(/spons/i):upward(a, .carousel-caption, .featurette, article)
forexgruppen.se##div[data-widget_type="image.default"] a:not([href*="forexgruppen.se"], [href^="/"]), .widget_media_image a:not([href*="forexgruppen.se"], [href^="/"])
forexgruppen.se##+js(noeval-if, adbEnableForPage)
forexgruppen.se,datormagazin.se,skogen.se##.cky-consent-container
forni.se##.recent-articles:has(.collaboration-brand)
forskning.se##.cli-modal
forstasidorna.se##body.tingle-enabled:remove-class(tingle-enabled)
forstasidorna.se##.tingle-modal--visible
forum.mustangclubsweden.org##a[href*="&do=advertisement&ad=1"]
forum.robsoft.nu##td[valign="middle"] > a[target="_blank"]
forum.robsoft.nu##.cookie-box
forvaltarforum.se##.ff_sponsored_articles, .widget_sow-image a[target="_blank"], .ff_banners_widget_widget
forvaltarforum.se##.ticker-title:has-text(/partner/i)
forvaltarforum.se##.ticker-title:has-text(/partner/i) + .mh-section
fotbolldirekt.se,hockeysverige.se,innebandymagazinet.se##.c-announcement:has(.c-label--sponsored)
fotbolldirekt.se,hockeysverige.se,innebandymagazinet.se##.c-announcement:has-text(/annons/i)
fotbolldirekt.se,hockeysverige.se,innebandymagazinet.se##.pdcw-item--code:has(img[src*="bet365"])
fotbolldirekt.se,hockeysverige.se,innebandymagazinet.se,motivation.se,fiskejournalen.se,alba.nu,padeldirekt.se,dagensopinion.se##.annons
fotbolldirekt.se,hockeysverige.se,innebandymagazinet.se,padeldirekt.se##.site-partnevisment, .h-background--sponsored-light, .row .text-center img, a[href^="https://hubs.la"], .c-partners, iframe[srcdoc*="_ad_div"], .annons-text
fotbollskanalen.se##a:has(.brand-info__ad-text)
fotbollskanalen.se##.brand, .desktop-ad-web, a[href*="telia.se/privat/tv/sport"] img, .mobile-ad-web, .ad-banner
fotbollskanalen.se##:is(.notice__tag_sponsored, .notice__tag):has-text(/sponsrat/i):upward(1)
fotbollsresultat.com##h2:has-text(Spel och dobbel) ~ p
fotbollsthlm.se##.fotbollsthlm-image-container:has(.fotbollsthlm-ad-link)
fotbolltransfers.com##div[class^="ad"], a[href^="https://ads."], .header_sponsored, .fresnel-greaterThanOrEqual-panorama, .fresnel-lessThan-panorama, a[rel*="sponsored"]
fotbolltransfers.com##div[style^="min-height"]:has(div[id^="fotbolltransfers_mpu"], div[id^="fotbolltransfers_mobil"])
fotbolltransfers.com##img[src*="/images/annonser/"]:upward(1)
fotbolltransfers.com##.smallNewsCategory:has-text(/sponsr/i):upward(.smallNewsLink)
fotboll-tv.se##.SMBoxContentBanner, a[data-gaevent*="action=bookmaker_odds"], #ouibounce-modal, .SMGameAtomSingleGameOddsComponent
fotboll.com##.header-static-lg, .fp-partner, .xs-ad, .bo-wrapper, #betsid, .news-banner-mini, .xs-cblock, .cookie_consent_bar, #odds, a.bellows-target[href*="/svenskaspel"], a.bellows-target[href*="/betting"]
fotboll.com,allsvenskan.se,superettan.se,swebbtv.se,hastnet.se##.smartbanner
fotosidan.se##+js(aeld, contextmenu, , showCopyrightBox)
fotosidan.se##.subArticlesponsored, div[style="width:300px;float:right;"], div[style="float:right;width:300px;"], #partner-box, .adbox-label
fotosidan.se,merinfo.se,allsvenskan.se,tasteline.com,jaktojagare.se,chefstidningen.se,realtid.se,norpan.se,moviezine.se,jaktjournalen.se,byggvarlden.se,omtanke.today,akademikern.se,socionomen.se##.ads
fragbite.se##.category:has-text(/spons/i):upward(article)
fragbite.se##.tn, .zooKeeper, #scraper, .subHeadSponsors
framtid.se###siteflash, #customer-link-container
fraser.nu##div[aria-label="Annonser"]
freeride.se##img[src*="/sponsor/"] + br + .boxlogo, .sidebar-front .boxen
freeride.se##.mark:has-text(/spons/i):upward(.post)
freeride.se##.sidebar-front .widget_text.dark ~ p
freeride.se##.visible-xs:has(a[href*="casino"])
freeride.se,gamereactor.se,happyride.se##.sponsor
fria.nu,stockholmsfria.se##[class*="annonser"], #cboxOverlay, #cboxWrapper
frihet.se##.CookieBar
frilagt.se##.elementor-location-header section.elementor-element:first-child
friluftsframjandet.se##[id^="ad-"]
funktionshinderpolitik.se##.topp-banner, .annons-mark
funnygames.se,nyckelspel.se##.slot-container
fuska.nu##span:has-text(/casino/i):upward(li)
fuska.nu##.list:has(a[href*="casino"])
fuska.se##.alert-success
futsalmagasinet.se##div.modal-cacsp-backdrop, div.modal-cacsp-position
futsalmagasinet.se##html.modal-cacsp-open:style(position:unset!important)
futsalmagasinet.se##span:has-text(/annonserat innehåll/i):upward(.td_block_wrap)
futsalmagasinet.se##.wp-block-column > h2:has-text(/annonser/i) ~ p
futsalmagasinet.se,newsvoice.se,obsid.se##aside.widget:has(a[href*="casino"])
fz.se##.article-facebook
fz.se##.card:has(.article-sponsored, a[href*="/sponsrat"])
fz.se##.fp-carousel .fpci-kicker:has-text(/^sponsr/i):upward(.fpc-item)
fz.se,fssweden.se##+js(set, adblock, false)
gaffa.se##a[href*="/annonser/"], a[href*="/sponsrat-"], div[id^="cncpt-"]
gaffa.se##h4:has-text(/sponsrade länkar/i):upward(.link-list)
gaffa.se##.article-overview__col:has(.gpt--loaded)
gamereactor.se##video:remove-attr(data-autoplay)
gamereactor.se###cookielawwarning, #eventad, [id^="sky"], [id^="ad_lead"], a[rel="sponsored"], .external_div_bigVideoAd, #mpu, #leftToLogo, .itsanad, div[class^="ad_Bumper"], div[style="min-height: 600px; margin-bottom: 20px;"], div[id^="ad_"], div[class^="preAd_"], div[class^="ad_smartphbig"], .adMobileBig, div[class^="preMobileBig"], .external_div_videoAd, .ad_mobilebigwrap
gamereactor.se###grtvbelt_Sponsored:upward(1)
gamereactor.se##+js(set, adblockEnabled, falseFunc)
gamereactor.se##.ad_interscroller:upward(.wrapper)
gamereactor.se##.colHomePlayer:has([data-slotads="videoad"]):remove()
garaget.org##+js(rmnt, #text, casino)
garaget.org##.gorgad, .gorg-side-content > div.small:nth-last-child(2), .gorg-side-content .bottom-buffer ~ *
gasetten.se##.footer-widgets .widget_block li
gasetten.se,fotbollsthlm.se##article:has-text(/är en annons/i)
gasetten.se,fotbollsthlm.se##.footer-links, .fotbo-target
gentlemannaguiden.com##.advertising, .sidebar .widget_text, .sidebar .widget_media_image, .has-post-thumbnail.category-okategoriserade
glassakademin.se##[class^="adverts-"]
gmfk.nu###site-preloader
godare.se##a p[class^="hyperion-css"]:has-text(INNEHÅLLER ANNONSLÄNKAR):upward(li, a.internal-link)
godare.se##h3:has-text(Annons):upward(1)
godare.se##.godare-ad-element, a[href*="/brand-studio"], a[href*="/brandstudio"], .recipe-ad, a[href*="utm_campaign"][data-test-tag="external-link"]
golfguidenonline.se###citadela-infobar
golflivet.se##a[href*="/annonssamarbete/"], .deals_block_wrapper, .ai-close-fit
golf.se##.partner-area
google.se##div.g:has(a[href*=".com.se/"]):has-text(/återförsäljare|rea|garanti|lågt pris|nöjd|priser|shop|bra pris|kläder|skor|outlet|frakt|butik|betala/i)
google.se##h2:has-text(Annons):upward(#topstuff)
google.se##mobile-promo
goteborgsgolfaren.se##.sgpb-popup-overlay, #sgpb-popup-dialog-main-div-wrapper, .et_pb_gallery
goteborg.com##body:style(overflow-y:initial!important)
goteborg.com##.cookie-popup, .overlay
grandtech.se##aside#secondary:has(.adsbygoogle)
grillbaronen.se##a[href*="/click."], #block-2, #block-4
grillbaronen.se##.post:has(a[href*="casino"], a[href*="kasino"], a[href*="betting"])
grillbloggen.nu##.rstbox
guideAds$xmlhttprequest,domain=barometern.se|blt.se|bt.se|kristianstadsbladet.se|olandsbladet.se|smp.se|sydostran.se|trelleborgsallehanda.se|ut.se|ystadsallehanda.se|vxonews.se|vaxjobladet.se|nsk.se|klt.nu
guldkanalen.se##div.grid_container[style*="height:240px;"]
gynning.net##.sponsored-notification:upward([id^="post-"])
hallakonsument.se##section[aria-label="Kakinformation"]
hallbartbyggande.com##div[id^="hallb-"]
hallbyhandboll.se,skiljebosk.nu##.cookiePush, .stickyFollow, .sponsorGroup__item
halsafitness.se,yogaworld.se,cyclingplus.se##h3:has-text(/samarbete/i):upward(.post-wrap)
halsafitness.se,yogaworld.se,cyclingplus.se##.sticky-sidebar, #gdpr-container, .slick-carousel
hammarbyfotboll.se##body[data-modal-open]:style(overflow-y:unset!important;)
hammarbyfotboll.se###seasonalTakeover, div[class*="sponsorBarContainer"], div[class*="footerSponsors"], .slick-slide a[target="_blank"]
handbollskanalen.se##.hb-adlabel, [id^="hb-"], .ad-placement-side, p > a[target="_blank"]
handelsnytt.com##.headerannons, .sidebarannonsseg, .footerannons
handel.ax###topadmob
hant.se,svenskdam.se##div.text-center:has(div[ad-placement])
happypancake.se##a[href*="casino"]:upward(1)
happypancake.se###__next > div > div.bar:first-child
happypancake.se##+js(aopr, Object.prototype.adUnits)
happyride.se##li:has(a[href*="/category/sponsrat/"])
happyride.se##.col-sm-4 > div[class]:has(a[href*="casino"], a[target="_blank"])
happyride.se,freeride.se##.anm1-container, [class^="anp"], [class^="ans"], .box.evergreen
hastnet.se##div[style*="--mobile-height"]:has(div[id^="div-gpt"])
hastnet.se##.add-wrap, .listings-search-ads, .right_panel, #pmg-widget-root
hbwebben.se##.elementor-widget-container > a > img
hd.se,sydsvenskan.se,allehanda.se,tidningenangermanland.se,arbetarbladet.se,avestatidning.com,bblat.se,dalademokraten.se,fagersta-posten.se,gd.se,lt.se,ltz.se,na.se,norrteljetidning.se,nynashamnsposten.se,op.se,salaallehanda.com,st.nu,tidningenharjedalen.se,vlt.se,falkopingstidning.se,jp.se,skaraborgslanstidning.se,skovdenyheter.se,smalandsdagblad.se,smalanningen.se,smt.se,tranastidning.se,vastgotabladet.se,vetlandaposten.se,vn.se,bandypuls.se,ljusdalsposten.se,ljusnan.se,soderhamnskuriren.se,ht.se,moratidning.se,borlangetidning.se,falukuriren.se,sodran.se,nyaludvikatidning.se,skd.se,nvp.se,nuiosteraker.se,hbl.fi,vastranyland.fi,bbl.fi##[class*="teaser-native"], lcl-ad, .ad-welcome, .affiliate-links__container, .x-bonnier-news-links__container
hejaolika.se##p[style^="text-transform"]:has-text(/annons/i)
hejaolika.se##p[style^="text-transform"]:has-text(/annons/i) + .wp-block-kadence-posts
hejaolika.se##+js(acs, advads_passive_placements)
hejaolika.se##[class*="partnerinfostyle"], div[id^="hejao-"], .kb-advanced-image-link[target], .category-partnerinformation, .kt-modal-linkalign-center, .hejao-target
hejauppsala.com##:is(div[class^="u-text"], h2):has-text(/^Reklam$/):upward(section)
hejauppsala.com,bredband.se##.cli-barmodal-open:style(overflow:auto!important)
helahisingen.se###custom_html-15, .code-block img, .banner-promotions-wrapper
helgon.se##[id*="banner"], a[href^="https://ad."], a[href^="https://ad2."]
hellofresh.se##a[data-test-id^="top-banner-ad"], div[data-test-id="exit-intent-banner"], div[data-test-id="urgency-banner-modal"]
hemhyra.se##.pageCookies, #ad-insider1, #ad-insider2, #ad-mobil-1, #ad-mobil-2, #ad-mobil-3, #ad, #ad1, #ad2, #adform-outstream, .ad__text, .entry__ad, .entry__related__sponsored, .module__sponsored
hemmafixbloggen.se##.post-item:has(.sponsor-summary)
hemmanytt.se###sa_slider_shortcode
hemmanytt.se##.annonsnotis + span + span + div.td-pb-row:has(a[href*="adtr.co"])
hemnet.se##body:style(overflow:unset!important)
hemnet.se##div[data-testid="living-cost-logos-section"]:has(span[aria-label="annons"])
hemnet.se##span:has-text(/annons från/i):upward(div[class^="ArticleContent_articlePage"])
hemnet.se###ad_unit_placeholder, div[class^="Panorama_panoramaAd"], .listing__panorama-banner, .broker-banner, div[class^="BrokerBanner"]
hemnet.se##:is(article, li):has([class*="SponsoredLabel"], .article-card__sponsored-text)
hemnet.se##:is(div[class^="Carousel"], #top_listing):has(div[class^="PaidPlacementLabel"])
hemnet.se##:is(small, span):has-text(/sponsrad/i):upward(article, li, a)
hemtrevligt.se##div[id^="hj-"], div[id^="ik-"]
hemtrevligt.se##.article:has(.annons)
hifitorget.se##.billboard-style, .between-posts
hifitorget.se##.row[style*="height"]:has(.adsbygoogle)
hippson.se##.main-article-container:has-text(/Sponsrad Artikel/i)
hitta.se##a[data-trackimp][target], .hitta-map .integration-txt, .section-details--alb, [class*="dummyAd"], [class*="StyledAdSlot"], [data-bind*="Ad"], div[class^="GraphicAd_"], [class*="adContainer"], [id*="_panorama"], [id*="_skyscraper"], div[style="min-height: 250px;"], div[data-track="displayplacering-customer"], a[data-test="boostAdLink"], div[class^="style_bannerContainer"], [data-track="click-promotion-banner"], div[class*="adWrapper"]
hitta.se##div[id^="hitta_mobile_"].placeholder:upward(div[class^="height"], div[class^="style_breakout"])
hitta.se##[class^="styleManual_mainContentBox"] > div[style^="min-height"]:first-of-type
hockeybladet.nu##.td_mod_wrap a img[data-permalink], a[data-wpel-link="external"][onclick], a.td-lazy-img[target], a[href*="casino"]
hockeybladet.nu##.vc_row_inner:has-text(casino)
hockeyettan.se##.club-ad-item, .banner-row
hockeyguiden.com##.main-loader.loader-bg
hockeymagasinet.com##body:remove-class(modal-open)
hockeymagasinet.com##gdpr-alert
hockeynews.se##.items-center:has(a[target="_blank"])
horisontmagasin.se##small:has-text(/annons/i)
hotellorestaurang.se,citymark.today,byggfakta.today###bannnerContainer, #pop_overlay, .banner-s, div.featured
hrnytt.se##article:has(.sponsored-article)
hrnytt.se##.banner-box
hrsvepet.se##.mini-title-link:not(.w-condition-invisible):has-text(/sponsra/i):upward(1)
hrsvepet.se,cfosvepet.se##.cookie-banner, .desktopbanner
humorbibeln.se,newsner.com,sportbibeln.se,ettgottskratt.se,djurbibeln.se##.inline-share-buttons
hungrig.nu##.ui-widget-overlay, .ui-dialog
husbilsplats.se##div[id^="husbi-"]
husvagnochcamping.se##div[id^="husvagnochcamping-"], .ast-below-header-bar
husvagn.se,husbil.se##strong:has-text(/samarbete/i):upward(li.item)
husvagn.se,husbil.se##.ui-top-adversite, #optin-cover, #optin
ibnytt.se##h3:has-text(Speltips):upward(.widget)
ibnytt.se##:is(a[href*="casino"], a[href*="speltips"]):upward(.widget)
icagruppen.se##div[ng-controller="CookieConsentCtrl"]
icagruppen.se##div[ng-show*="isUiDisabled"]
ica.se,naringslivetvgl.se,dalarnasaffarer.se,stockholmsaffarer.se,jamtlandsaffarer.se,hallandsnaringsliv.se,sjuharadsnaringsliv.se##.banner-area
idrottensaffarer.se###header:style(height:unset!important;)
improveme.se##.banner-center, .banner-center ~ br, div[class^="ad-container"]
improveme.se##.flow_teaser:has(a[href*="casino"], a[href*="poker"], a[href*="cbd-olja"])
improveme.se##.wp-pagenavi:style(position:unset!important;z-index:unset!important)
inblick.se##div[class^="ads"]
indien.nu##.nyhetsochreseartiklar .views-row:has-text(/casino/i)
industrinyheter.se,dagensnaringsliv.se,infrastrukturnyheter.se,sportochfritidsnyheter.se,inredningsnyheter.se,byggnyheter.se,dagensfastigheter.se,stockholmsbyggnyheter.se,energinyheter.se,vindkraftsnyheter.se,solenerginyheter.se,jarnvagsnyheter.se,transportochlogistik.se,metallerochgruvor.se,papperochmassa.se,miningmetalnews.com##.insider-ads, [id^="mainadvertorial"], [id^="dfptag"], .block-advertorial, .block-views-blockconventus-info-articles-info-article-block, #dfp-tag-before_artikel, #dfp-tag-mobile_before_artikel, #block-views-block-leader-article
industritorget.se###pnlCookie, .campaign-top, .campaigns-right
inet.se##+js(set-cookie, allow-marketing-cookies, 0)
influens.se##strong:has-text(Annons:):upward(.code-block)
influens.se##.code-block-label:has-text(Annons:)
influens.se##[class*="ai-viewport"], .ai_widget, #cb-sidebar-h, .livewrapped, .livewrapped_mobil
ingenjorsjobb.se##body:remove-class(advert-take-over-active)
ingenjorsjobb.se##.advert-take-over
inkopsradet.se##div[id^="inkop-"]
innebandy.se##[class*="banner-container"], .sponsorsswipeblock
inredningsarkitektur.se##.article:has-text(/sponsrad artikel/i)
internetmedicin.se##[itemtype="https://schema.org/WPAdBlock"]
internetodontologi.se##.overlay
internetodontologi.se##+js(aeld, /contextmenu|keydown/, e.preventDefault)
ipo.se##.tag-sponsrad
itseniorerna.se###astroid-preloader
itseniorerna.se###redim-cookiehint-modal
it-finans.se,it-halsa.se,it-kanalen.se,it-pedagogen.se,it-retail.se,it-hallbarhet.se##a[onclick^="gtag"], .header-banner, .penci-featured-cat-custom-ads
it-finans.se,it-halsa.se,it-kanalen.se,it-pedagogen.se,it-retail.se,it-hallbarhet.se##.widget-title:has-text(/annons/i):upward(aside)
it-finans.se,it-halsa.se,it-kanalen.se,it-pedagogen.se,it-retail.se,it-hallbarhet.se,espressomedia.se##.penci-wrap-gprd-law
jaktjournalen.se##.activate-notifications-container.shown, .newsletter-popup-content-overlay, .newsletter-popup, [class*="ai-viewport"]
jaktjournalen.se##.post:has(.post__category--sponsored)
jaktojagare.se##div.cookie-warning-container, .mb-adarea
jaktplay.se##.jaktplay-ad
jaktsidan.se,edgeflyfishing.com###ipsLayout_mainArea > iframe
jarnvagar.nu##.et_pb_module:matches-css(before, content: "Annons:")
javligtgott.se##div[id^="ad-panorama"]:upward(.elementor-section)
javligtgott.se##.jet-popup
jobsinsweden.se##+js(set, eazy_ad_unblocker, null)
journalisten.se##.o-blockCarousel--placementAd, .o-blockArea__item--block-ad, .m-blockAd
kalender.se##.day-nav ~ a:not([href*="kalender.se"]), a:not([href*="kalender.se"]) img, div[style^="height:340px"], div[style^="height:110px"]
kalmar.nu###rb-cookie
kamrat.com###kadDiv, div[style="margin:25px 0;max-width:255px!important;"], #scrollAdj ~ *
kamrat.com##+js(set, showAds, false)
kamrat.com##+js(set, trap, noopFunc)
kardemummagumman.se###custom_html-2
karinrahm.se##.thb-page-transition-on:style(opacity:1!important)
karlskogavaxer.se##.elementor-heading-title:has-text(/annons/i):upward(.elementor-column)
karriarlakare.se##a:has(.annons-label)
karriarlakare.se##a[target][onclick], #cliSettingsPopup
karriarlakare.se,livinguppsala.se,battrestadsdel.se,butikstrender.se,forskning.se,vardfokus.se,varvat.se,smaspararguiden.se,aktuellsakerhet.se,maklarvarlden.se,kvartal.se,sjostadsbladet.se,tidningenridsport.se,cookaholic.se,vinliv.se,raa.se,svenskfilmdatabas.se,hejaolika.se,arbetsvarlden.se,hockeybladet.nu###cookie-law-info-bar
kartor.eniro.se##.e-banner
kb.se,dansportalen.se,hh.se##body:style(overflow:unset!important; position:unset!important;)
kb.se,dansportalen.se,hh.se##.sv-marketplace-sitevision-cookie-consent, .sv-cookie-consent-modal, .env-modal-dialog__backdrop, .env-modal-dialog__backdrop--in
kiacarclub.se##.forumlist-main-inner > div[style]
kiacarclub.se##.sidebar-block:has-text(/annons|sponsor/i)
kimura.se##a[href*="unibet.com"], a[href*="/kampanjer."], a[href*="utm_campaign"], div[class^="yw-"], a[data-wpel-link="external"][target="_blank"]
kingsizemag.se##a:has(.disclaimer-tag-img)
kingsizemag.se##div#video-overlay, div.sidebar_frame, #affiliates, #affiliates + .text, #popup-interstitial-overlay, .cu_banner, #interstitial-overlay, .kingsize-native
kittad.se##li:has(.kittad-label-sponsored)
kittad.se###header-top, div[data-hook="consent-banner-root"]
klart.se##body:remove-class(mega-loading)
klart.se##div[id^="sp_message_container"]
klart.se###overlay, a[rel*="sponsored"], .-panorama-ad-wrapper
klimatnytt.se##.tm-cookie-banner
knulla.se###cookie-popup
kobe.se##p:has-text(/annonser:/i):upward(.widget_block)
kobe.se##.post:has(a[href*="casino"])
kokaihop.se##body:style(overflow-y: auto !important;)
kokaihop.se##.ads-wrapper-main, .InterstitialModal
kokaihop.se##.cookieBarWrapper:remove()
koket.se##[class*="carousel_sponsored"]:upward([class*="carousel_item"])
koket.se##[class*="list_item_sponsored"], [class*="promotion_bottom_holder_wrapper"], [class*="beverage-recommendation_wrapper"], [class*="list_item_wide_sponsored"], [class^="ad_position"]
koket.se##[class*="sponsorLabel"]:upward([class*="mosaic_item_wrapper"])
kolla.tv##div[style^="position: fixed; left: 0px; top: 0px; width: 100%; height: 100%; z-index: 999;"]
kollega.se##.block--gamw
kolozzeum.com##td[width="305"], br + a[href*="/casino"]
kompanjoner.se##.site-loader
komponentkoll.se##.gdpr-wide
konsumentmagasinet.se##.pricerunner
kristendate.se##div[id^="adv"]
kristendate.se##.cc-banner.cc-bottom
kritiker.se##div.recad, div.adhor, div.stickyad
kritiker.se##iframe[allow]:remove-attr(allow)
kritiker.se##+js(set, checkAdblocker, noopFunc)
kritiker.se##+js(set, checkAdsBlocked, noopFunc)
kritiker.se##+js(set, premium, trueFunc)
kritiker.se##+js(set, p, true)
kulturama.se##.CookiePopup
kulturbloggen.com,schack.se##.sidebar .widget_custom_html
kultwatch.se##.js-preloader > .document, .js-preloader > .hero-section:style(opacity: 1 !important; visibility: visible !important;)
kurera.se##.pc-das, .newsletter-popup
kvalitetsmagasinet.se,miljo-utveckling.se,telekomidag.se,vdtidningen.se##article:remove-class(closed)
kvalitetsmagasinet.se,miljo-utveckling.se,telekomidag.se,vdtidningen.se###subscribe_splash, [class*="nativeadwidget"], .partnermedia, .annonswidget
kvartal.se##.email-popup-wrapper
kvartal.se##.square-format:has(.kv-ad-label)
kwiss.me##.square-item:has(.qz-quiz-sponsored)
lajvo.se###panoramaTop
lajvo.se##.postCard:has-text(/bonusar|casino|betting|spelbranschen/i)
lakartidningen.se##.screen-sm, .screen-md
lakartidningen.se,hockeynews.se,canariajournalen.se##.advertisement
landleyskok.se##.inpostbanner, .banner-leaderboard
langd.se##.single-entry__ads
lantbruksnytt.se###startpage-top-right, .ads_text + a, div[class*="square_rotate"], a[target="_blank"][rel="nofollow"], #ouibounce-modal
laromedia.se##img[alt="Annons"] + .img-flipper
lawline.se##[class^="CookiesModal"]
lchfarkivet.se##.lchf-modal--wrapper, div#beskrivning[style="font-size: 10px; text-align: center; color: #8E8C8C; max-width: 700px;"]
lektionsbanken.se,runnersworld.se##.footer-newsletter
lesscarbs.se##article:has(a[href*="/annonssamarbete/"])
lesscarbs.se##.elementor-image > a:not([href*="https://lesscarbs.se"]), a[href*="/affiliates/"], div[id^="1"][style*="250px"]
lesscarbs.se##.e-loop-item:has(div[data-eael-wrapper-link*="annonssamarbete"])
lesscarbs.se#@#.category-annonssamarbete:not(body):not(html)
leta.se###bookingcom-resor-wrapper, #aktuellaerbjudanden, #sky-left-wide, .topNavItem[href*="casino"], .topNavItem[href*="betting"], #bottom-splinks
levandehistoria.se##div[class^="CookieBar"]
lexbase.se##+js(cookie-remover, lmt)
lidingonyheter.se##.moban
lifeofsvea.se,quizza.nu,trendenser.se##.cookie-info
lindasbakskola.se,jennysmatblogg.nu,zeinaskitchen.se,filippoon.se##.panorama-sticky, .sticky-area, #ad-outofpage_dynamic
lindasbakskola.se,skk.se,realtid.se,viivilla.se,ungdomsfotboll.se##a[href*="/bit.ly/"]
linguee.se##div[class*="ad_container"], div[class*="_ads_"]
lira.se###cookies-accept
lira.se,danstidningen.se,slangopedia.se,tidningen.se###ads
listor.se##article.feed-item:has-text(/låna pengar|casino|betting/i)
listor.se##article:has(a[href*="/annons/"])
listor.se###ss-floating-bar, .top-ads-widget, .header-inner center, #sidebar-right .widget_custom_html
listor.se##:is(a[href*="casino"], a[href*="betting"], a[href*="poker"]):upward(.elementor-widget)
litteraturmagazinet.se###pageContainer > div:first-child:not([id]), #topContainer a:not([href="/"], a[href="/sitesearch"])
livesport.expressen.se##[class^="BauProvider"]
livetochdiabetes.se###text-3
livetsgoda.se##body:style(opacity:unset!important)
livetsgoda.se##.penci-rlt-popup
livetsgoda.se,betongforeningen.se,espressomedia.se,realtid.se,ordfrontmagasin.se,europaportalen.se,motorsportbladet.se,battregolf.se,nitroz.se,magasinethockey.se##a[target$="blank"] img:not([class^="tweet"])
livinguppsala.se##.fusion-post-content-container:has-text(/^annons/i):upward(article)
livsmedelsverket.se###CookieConsent
livsmedelsverket.se##.lock-scroll:style(overflow:unset!important)
livsstil.se##article:has(.ad)
livsstil.se##a[href*="campaign"][data-test-tag="external-link"], div[data-ad-subtype], [data-test-tag="prisjakt-carousel"]
livsstil.se##div[data-variants*="article-panorama"]:upward(1)
livsstil.se##h3:has-text(/^Annons$/):upward(1)
livsstil.se##p:has-text(/^kommersiellt innehåll/i):upward(article)
livsstil.se##p:has-text(/^kommersiellt innehåll|^annons$/i):upward(a)
livsstil.se,godare.se##[id^="adPlacement"]:upward(1)
ljudochbild.se##div[class^="col-md"][style*="border-radius"]:has(a[href*="/advertorial"])
ljudochbild.se###MoreLink_content-container:style(height:unset!important;)
ljudochbild.se###MoreLink_fade-out-div
ljudochbild.se##.adremark, .coofad, .popup-overlay, .hidead, .phoneads, .pricecomp, .offerz, .type-articleadvertorial, .adblock, .lbplussinfo, .popup-overlayx, a[href*="/advertorial"], a[href*="/advertorial"] + .textbox, .prisjakt, #stickleft, #stickright
ljudochbild.se##.thecontent, .entry-content:style(max-height: unset !important; overflow: initial !important; height: unset !important;)
ljudochbild.se##.wp-caption:style(display:initial!important)
ljungbysporten.se##section.widget_media_image, a[target="_blank"]:not([href*="ljungbysporten.se"])
ljuskultur.se##body.private:remove-class(private)
ljuskultur.se,bettips.se,spelo.se,skogsaktuellt.se,maskinbladet.se,entreprenadaktuellt.se,ja.se,husbilhusvagn.se,klassiker.nu,mopedgaraget.se,vibilagare.se,caroftheyear.se,automobil.se,endurobloggen.se,riksettan.net,fightermag.se,frillesasbandy.se,dh.se,djungeltrumman.se,skik.se,omni.se,campingsverige.se,eniro.se,svenskjakt.se,realtid.se,restaurangvarlden.se,naringslivetvgl.se,dalarnasaffarer.se,stockholmsaffarer.se,jamtlandsaffarer.se,hallandsnaringsliv.se,sjuharadsnaringsliv.se,nyheteridag.se,epochtimes.se,alekuriren.se,omniekonomi.se,sverigesindustri.se,onkologiisverige.se##.banner
ljuskultur.se,hrnytt.se,aapl.se,inredningsarkitektur.se,inblick.se,matklubben.se##.cookies
lokalguiden.se##.applicant-match-container, .banner-item
lokalnytt.se##.panoramaImageBox
lokalti.se##:is(img[src$="a_top.png.webp"], a[href*="casino"]):upward(section.elementor-section)
loppi.se##a[href="https://loppi.se/promotion"]:upward(.page__section)
loppi.se##.entry__teaser--promotion, .wpcnt, .sunt-widget, .lifeofsvea-widget
lovelylife.se##.elementor-image a[href]:not([href*="lovelylife.se"]) img
luleahockeyforum.com##main > div:first-child:has(.banniere)
lundagard.se###bdCheckAlso.bdCheckAlsoShow, .topBanner, #sidebar .widget_media_image
lundextra.se,huddingeextra.se,sundsvallextra.se,goteborgextra.se,sollentunaextra.se##.category-partners
lundgiants.se##.cookieAlert
lundgiants.se##strong:has-text(Detta är en annons):upward(.inner)
lundgiants.se###LoggaDiv:style(position:unset!important;)
lwcdn.com##+js(aeld, /^(?:adBlocker|contextmenu)$/)
lwcdn.com,alingsastidning.se,bohuslaningen.se,gp.se,hallandsposten.se,hn.se,stromstadstidning.se,ttela.se,kungsbackaposten.se,kungalvsposten.se,molndalsposten.se,partilletidning.se,sttidningen.se,markposten.se,harrydaposten.se,mellerudsnyheter.se##+js(json-prune, autoplay players.*.ga acl.ads players.*.autoplay)
lysekilsposten.se###archiveAdContainer, .casino-wrapper
m3.se,pcforalla.se,macworld.se##span:has-text(/sponsr/i):upward(article)
m3.se,pcforalla.se,macworld.se##+js(href-sanitizer, a[href*="/idg.digidip.net/"], ?url)
m3.se,pcforalla.se,macworld.se##.amazon_lightning_deals_wrapper
mabra.com,motherhood.se##article.grid:has-text(/annonssamarbete/i)
macken.xyz##a[target="_blank"]:not([href^="/"]):not([href*="/macken.xyz"])
macken.xyz##.et_pb_section:style(opacity:1!important; animation-duration:unset!important; animation-fill-mode:unset!important;)
magasinetparagraf.se###large_banner
magasink.se##[data-magasintrackbid]
maipenrai.se##.cWidgetContainer > ul > li:first-child, div[style*="border: 1px solid"] a[target="_blank"], div[data-role="sidebarAd"], a[href*="&ad="]
maklarvarlden.se##article:has(.sponsored-inlist)
maklarvarlden.se##.hustle-popup
maklarvarlden.se##.td-post-category:has-text(/spons/i):upward(2)
maklarvarlden.se##.td-pulldown-size:has-text(/spons/i):upward(3)
maltermagasin.se##.mh-sidebar, .mh-header-columns
maltermagasin.se##.widget_media_image:has-text(/annons/i)
maringuiden.se##.banner_hoger, .google_ads_mg_frontpage, .footerComercialDiv
marknadschefer.se##section.elementor-inner-section:has(.adsbygoogle)
marknadschefer.se##.elementor-column:has(.ekit-sticky)
marknadschefer.se##.elementor-widget-heading:has-text(/Sponsra|annons/i)
marknadschefer.se##.elementor-widget-heading:has-text(/Sponsra|annons/i) + .elementor-widget-post-block
marsta.nu##.outsider, .panel--naringsliv
matinspo.se##div:remove-class(with-ads)
matinspo.se##[id^="matin-"]
matkanalen.se###sidebar .widget_text
matmalin.se##div[id^="matma-"]
matochpyssel.nu##.loading:style(opacity:1!important)
matpriskollen.se###kd-preloader
matspar.se##div[style="z-index: 2000;"],div[style="z-index: 2000;"] + div
matspar.se###ad-panorama-category:upward(1)
matspar.se##+js(json-prune, payload.ads campaigns.*)
matspar.se##.overflow-hidden:style(overflow-y: initial !important;)
medibok.se##noscript:has-text(mdp-deblocker-js-disabled):remove()
medibok.se##style:has-text(body * :not):remove()
medibok.se##+js(acs, show_msg)
medibok.se##.annonsmellandiv, .annonssidadiv
megafonen.se##[data-article-sponsored="true"], .content-main-adwrapper, .campaign-sidebar
meningokockfonden.se###page_preloader
merinfo.se##article[data-customer]
mestmotor.se##.advInsideSticky
mestmotor.se##ul.wp-block-post-template:has(a[href*="/kategori/partner/"])
metalcentral.net##.bannergroupno-padding
metalcentral.net,egoinas.se###tm-top-a
metalcentral.net,rotter.se##.bannergroup
metromode.se##+js(href-sanitizer, a[href*="metromode.se/bouncer"], ?url)
metromode.se##.advert:upward(.slick-item):remove()
metromode.se##.b-topshop
metromode.se##:is(.b-card, .b-related__item):has(.advert)
mhis.se##.bg-grey-light:has(a[target="_new"])
milansverige.se##.elementor-image a[target="_blank"], .oc_cb_wrapper, .elementor-widget-image a[target="_blank"]
miljomat.se##[id^="Annons"]
minhembio.com##div[style="height: 120px;"]:not([id]):not([class])
minimalisterna.se##p:has-text(/i samarbete med/i):upward(.post)
missatsamtal.se##.nosnaj
missatsamtal.se##.comment:has(.nosnaj)
mitti.se##h3:has-text(/annons/i):upward(.image-component-unprocessed)
mitti.se###cruncho_now_iframe:remove()
mitti.se##+js(set, NWS.config.enableAdblockerDetection, false)
mitti.se##.profile-native
mitti.se,cafe.se,praktisktbatagande.se##+js(aeld, scroll, helpers.scroll(id))
mmabetz.se##.desktop-homepage-ad, .desktop-main-ad, .latest-betting-campaigns, .best-casino-section, .top-casino
mmanytt.se##.front-banner, .front-banner-cover, #text-2, [class*="sponsrat-inlagg"], a[href*="://kampanjer."], .ohmbet_link, a[href*="adsrv.eacdn.com"], .jeg_postblock + .wpb_content_element, .spelbolag-text, .adbox, .fight-odds-aggressive
mmanytt.se##.img-featured-posts-image:has(a[href$="/annons/"])
mmanytt.se##.tablepress:has(a[href*="expekt"])
mobilanyheter.net##a[href*="rocketpot.io"], a[href*="casino"], a[href*="betting"], .a-wrap
mobilanyheter.net##+js(set, ai_run_scripts, noopFunc)
mobil.se,kamerabild.se##a[href^="/partner"]
mobil.se,kamerabild.se##.markupbox:has(a[href*="casino"])
modernalivet.se##body.modal-active:style(overflow:unset!important)
modernalivet.se##h3:has-text(/annons/i):upward(.sidebar-widget)
modernalivet.se##.excerpt:has-text(/annons/i):upward(article)
modernalivet.se##.modal-wrap, .slide-in-box
modette.se##.true_native_block
morotsliv.com##.et_bloom .et_bloom_flyin_center, a[href*="/?utm_medium=affiliate"], a.bigblue[target]
motivation.se##.card:has(.sponsored)
motivation.se##.sponsored-item, [class*="banner"], .outsider
motormagasinet.se,dagenshandel.se,food-supply.se,plastnet.se,habit.se,woodnet.se,foodnet.se,transportnet.se,processnet.se,packnet.se,verkstaderna.se,medtechmagazine.se,recyclingnet.se,rt-forum.se,uochd.se,lifesciencesweden.se,fri-kopenskap.se,cleannet.se,framtidensbygg.se,entreprenad.com,metal-supply.se##.box-of-announcement, a[href*="campaign"][target="_blank"], div[class*="rotating-"], #bottombanner, #promoPopup, .modal-backdrop, .newsletterPopUp
motorsportbladet.se##:is(article, li):has(a[href*="casino"], a[href*="kasino"])
moviezine.se##strong:has-text(ANNONS:)
moviezine.se###home_ans, [name="article-advertisment"]
moviezine.se##.inner_article:has-text(/sponsrat|annons/i)
mygatemagazine.se##.textwidget:has-text(Annons)
mytaste.se##body.modal-active.modal-open::before, body.modal-active::before:style(opacity: unset !important; content: unset !important;)
mytaste.se##div[id*="panorama_"], [class^="affiliate-container"], .site-header__panorama, .alert-cookiedisclaimer
mytaste.se##.recipe-modal[data-state=default] .modal-container.open, .recipe-modal[data-state=panorama] .modal-container.open:style(padding-top: 0 !important;)
mytaste.se##.site-wrapper[data-state=panorama], .site-wrapper[data-state=default]:style(padding-top: 40px !important;)
mytaste.se##[id^="Modal_plugin"]
m.yelp.se##div[class^="overlay-color-cohort"]:has(a[aria-label="Download the Yelp app"])
m.yelp.se##html:style(overflow:unset!important; position:unset!important;)
naringslivetvgl.se,dalarnasaffarer.se,stockholmsaffarer.se,jamtlandsaffarer.se,hallandsnaringsliv.se,sjuharadsnaringsliv.se###dr-preloader
naringslivetvgl.se,dalarnasaffarer.se,stockholmsaffarer.se,jamtlandsaffarer.se,hallandsnaringsliv.se,sjuharadsnaringsliv.se##.header-menu__wrapp:style(position:unset!important)
naringslivetvgl.se,dalarnasaffarer.se,stockholmsaffarer.se,jamtlandsaffarer.se,hallandsnaringsliv.se,sjuharadsnaringsliv.se##.header-top__wrapp, .article-item__banner
naringslivetvgl.se,dalarnasaffarer.se,stockholmsaffarer.se,jamtlandsaffarer.se,hallandsnaringsliv.se,sjuharadsnaringsliv.se##.list-article__item-inscription:has-text(/sponsrat innehåll/i):upward(.list-article__item)
naringslivetvgl.se,dalarnasaffarer.se,stockholmsaffarer.se,jamtlandsaffarer.se,hallandsnaringsliv.se,sjuharadsnaringsliv.se##:is(.slick-slide, .article-item__line-bottom):has(.sponsored-badge)
naringslivetvgl.se,dalarnasaffarer.se,stockholmsaffarer.se,jamtlandsaffarer.se,sverigesindustri.se,hallandsnaringsliv.se,sjuharadsnaringsliv.se,onkologiisverige.se##.cookies-popup
narkive.se##div[onimpression]
nasdaqomxnordic.com##+js(acs, $, shuffle)
naturvetarna.se##.Advertisement
netdoktor.se,netdoktorpro.se##.article-list__item__link--sponsored, .ispanorama, #Popup, .ElementAdvertisement
netflixguiden.se##div.lboard, div.instream-dynamic, #top-area-promo, div.sidebar div.sticky, .promo, .lboard-desktop, .lboard-mobile, #bottom-sticky-promo
news55.se##div.container:has(a[href="/author/news55-partner/"])
news55.se##div.justify-center:has(div[id^="news55_pano"], div[id^="news55_tws"], div[id^="news55_mobil"])
newsner.com,humorbibeln.se,sportbibeln.se,ettgottskratt.se,djurbibeln.se###wsfb-container, .share-buttons, .ad-space
newsner.com,humorbibeln.se,sportbibeln.se,ettgottskratt.se,djurbibeln.se##.ssp_divider:has(.sponsored-bar)
newsvoice.se##h3:has-text(/annons/i) + .textwidget
newsvoice.se##.sponsrad, .sponsradcol1
ng.se###nativendo-mainfeed:upward(1):remove()
ng.se##.secondary-sidebar > .panel-pane:last-child
ng.se##.view-partner-articles, [class*="sponsored-article"], .tertiary-bottom, div[class*="nojesguidenads"]
nogg.se##:is(td[rowspan="2"][align="left"], table[width="640"][cellpadding="7"]):has(a[href*="casino"])
nordfront.se##span:not(.post-content):has-text(/annons/i):upward(.post)
nordfront.se###campaign_area
nordichardware.se##span:has-text(/sponsrat/i):upward(.td_block_wrap)
nordichardware.se##.pspy_info, [class^="prisjakt-"]
nordichardware.se##.td-big-grid-post:has(a[href*="/sponsrat/"])
nordiskradio.se###cookieWindow
nordiskskog.se##.templateHelannonsBOX
norrahalland.se##.bannercontent
nouw.com##.washer.loaded.displayed
nouw.com##.badge:has-text(/annons/i):upward(li)
nyadagbladet.se##.third-col, article[class*="sponsrad"], div[id^="nyd-"], .below_header_front_page, div[data-aeon-news-trackbid="1"]
nyadagbladet.se##.widget_media_image:has-text(/annons/i)
nyadagbladet.se,ff.se,rocknytt.net,magasink.se,evergreengarden.se,butikstrender.se,mykitchenstories.se,transportnytt.se,inpress.com##.elementor-popup-modal
nyan.ax##.gdpr
nyan.ax##a[onclick*="banner"]
nyatider.nu##section.dce-visibility-event:has(a[href*="casino"])
nyatider.nu##.elementor-popup-modal:has(a[href="/integritetspolicy"])
nyatider.nu,autonytt.se##[href*="casino"][target]
nyfiknainvesterare.se##article.post:has-text(/annons från/i)
nyheter24.se##.breadtext_content.paywall_breadtext p:first-child::before
nyheter24.se##.lazyload_bar.show, .lazyload_outer.show, .sponsrat, .is_native, .sticky-scroll, .flow_ad
nyheteridag.se##article:has-text(/sponsrat innehåll/i)
nyheteridag.se##h2:has-text(/samarbetslänkar/i):upward(.article-inner)
nyheteridag.se##li:has(a[href*="kasino"], a[href*="casino"], a[href*="-slot-"])
nyheteridag.se##.widget.facebook, .content > div:not([class]) img, a[href*="www.casino"], a[href="/karnkraft.php"]
nyhetersto.se##.site-branding a ~ p, .wp-block-jetpack-slideshow
nyhetsbyranjarva.se##div[style="display: flex; justify-content: center; flex-direction: column; align-items: center;"]
nyhetsbyranjarva.se,nyan.ax,tv-kanal.se,golfguidenonline.se##.g
obosdamallsvenskan.se,elitettan.se##.rmss_ap-top-ad + .rmss_t-ap-grid-stripe:has(a[href*="svenskaspel"])
obosdamallsvenskan.se,elitettan.se##.rmss_module-sponsors, .rmss_ap-top-ad, .rmss_ad-panorama, .rmss_t-momenu__sponsors-area
obsid.se##a[href*="casino"]
offside.org###opab-modal, .opab-footer-offer
omnihalsa.com,skanesport.se,sportpanelen.se##.stream-item
omni.se,omniekonomi.se##div.group:has([class*="sponsoredcluster"])
omni.se,omniekonomi.se##.article--sponsored, .resource--sponsored, .component--sticky-sponsor-banner, .pre-banner, .banner--toppanorama, .banner--midpanorama, .group--banner
omni.se,omniekonomi.se##.header-banner--regular, .app-banner:style(--banner-offset: 0 !important;)
omni.se,omniekonomi.se##.resource--link:has(a[href*="article-ad-"])
omtanke.today##.featured
omvarlden.se,skolvarlden.se##.cookieControl
opulens.se##.mailpoet_form, #secondary
ordbokpro.se##+js(set, ab_disp, noopFunc)
ordfrontmagasin.se##.oc_cb_wrapper, .simple-image a:not([href^="/"]):not([href*="ordfrontmagasin.se"])
ordguru.se##.visible-lg, .hidden-lg
orebronyheter.com###top-wrapper
oru.se##.modal-cookieform
oru.se##.no-scroll:style(overflow: initial !important;)
oskarshamns-nytt.se##article.category-shoppingguide
oskarshamns-nytt.se##:is(.adsbygoogle, a[href*="casino"]):upward(.elementor-section)
osterbottenstidning.fi,sydin.fi,vasabladet.fi##.online-teaser--advertorial, .online-ad-container
padeldirekt.se##.article-row:has(.h-background--sponsored)
padeldirekt.se##.c-featured-article:has(a[href*="/sponsrat"])
padeldirekt.se##.text-center:has(div[id^="padeldirekt"])
padelfeber.se##.pfm-partners, .pff-partners, .c-widget-ad, .c-teaser--native, #toBanner
pakryss.se##div[id*="ad_banner"]
pilsner.nu##.overlay-loader
pilsner.nu##:is(.et_pb_fullwidth_image, .et_pb_image) a:not([href^="/"]):not([href*="pilsner.nu"]), .mctb-position-bottom
piraja.se###panoramaholder, #parallax, .cc-floating, a[href*="utm_medium=banner"]
piraja.se##:is(.intro, #hero, #featholder):has(.spons)
pirkt.se##aside#below-header, aside.sidebar-right img, aside.sidebar-left img, aside#above-main, aside#after-first-post, h1 + .wp-block-video, h2 + .wp-block-image img[src$=".gif"]
placera.se##.noMarginAd
placera.se##a:has-text(/^annons/i):upward(.section)
plastikoperationsforum.se,riksettan.net,automobil.se,endurobloggen.se,vibilagare.se,mopedgaraget.se,caroftheyear.se,klassiker.nu,alandsradio.ax,svjt.se,so-rummet.se###sliding-popup
playradio.se##.sidealtcol
podcasts.nu##.sponsor-list, .cookie-law-wrapper, .big-ad-placeholder, .affiliate-wrapper
poddtoppen.se##.txs-a
podtail.se##aside a[href*="utm_campaign"]
podtail.se##.item-list__item:has-text(/annons från/i)
pomu.se##[class^="Banner"]
poolforum.se##div.adfit, .cookie_notice, div[style^="width:100%;max-width: 728px;"] > div[align="center"], div[style^="width:100%;max-width: 728px;"] > br
popularastronomi.se##a.gofollow[data-track]:not([href*="www.popularastronomi.se"])
pressbladet.se,svenskpress.se,foretagsbladet.se,gestrikemagasinet.se,cfanytt.se,lasarnas.se,hembostad.nu,sportidrott.se,nojesmagasinet.nu,halsasverige.se,mandarinmedia.se##.isax, #cookiebar
pricerunner.se##span:has-text(/sponsra/i):upward(div[class$="Container-root"])
prisjakt.nu##.pjra-relative
proshop.se##body:style(background-image: none !important;)
proshop.se##.site-background-banner
pussad.se##html.g1-popup-visible:style(overflow: initial !important;)
pussad.se##.g1-popup-newsletter, .g1-slideup-wrap
quizza.nu###takeover
qx.se##.qxa-container
racenews.se###block-2
radiotreby.se##.mobileHide, .mobile-show
radio.se##:is(a[data-testid="region-tag"], a[data-testid^="taglist-item"]):style(background-image:none!important; background:rgb(2,114,140)!important;)
radio.se##:is(.md\:min-h-\[90px\], .lg\:min-h-\[250px\], .h-\[250px\], .justify-between.md\:mx-10):has(div[id^="RAD_D"], div[id^="RAD_M"])
ratsit.se##.promo
ravarumarknaden.se###header > div > div.last, #block-4, #mvp-leader-wrap
realtid.se##.link:has(.meta--add)
realtid.se##.realtid-add, .realtid-ad, .infinite-scroll.native-wrapper
recepten.se,foreca.se###topBanner
recept.se##div[class*="ad-wrapper"], button#cookiePreferences, .c-modal-backdrop--active
rejsa.nu###adsblock, #adsblockfoot, .fpright, div[onclick*="window.open"]
reseguiden.se##.adsbox-wrapper, .banner-xxl_panorama-container, .banner-top-container
restaurangvarlden.se##.banner-col, .alt-banner-col
res.se##.res-display
ridsport.se##.svrf__sticky-ad, .svrf-block__banner, .sv-cookie-consent-banner, .sp-banner-block, .sp-double-ad-block, .sp-head-sponsor-container, .sp-regular-sponsor-container
riktighockey.se###custom_html-2
rocknytt.net##[data-widget_type*="bnnrwidgets"], a[href*="/annons/"], div[data-widget_type="image.default"] a[target="_blank"]
rodeo.net##article[data-section="allmänt"]
runnersworld.se##.post-card-sponsored, .modal-plus, .modal-backdrop
runnersworld.se,motormagasinet.se,dagenshandel.se,food-supply.se,plastnet.se,habit.se,woodnet.se,foodnet.se,transportnet.se,processnet.se,packnet.se,verkstaderna.se,medtechmagazine.se,recyclingnet.se,rt-forum.se,uochd.se,lifesciencesweden.se,fri-kopenskap.se,cleannet.se,metal-supply.se,framtidensbygg.se,entreprenad.com,branschstegen.se,skogsforum.se,bio.se##.modal-open:style(overflow:initial!important)
runnersworld.se,utsidan.se,hockeymagasinet.com,driva-eget.se,foretagande.se,revisionsvarlden.se,travelnews.se,mittforetag.com##.sponsored
sakochliv.se##+js(acs, checkCampaignCookie)
sakochliv.se##.cookie-disclaimer-wrap, .type-promo, .sector-annons
samfalligheterna.se##.tdm-popup-modal-wrap
samfalligheterna.se##.tds-locked-content:style(display:unset!important;)
samfalligheterna.se##.tds-locked-content[hidden]:remove-attr(hidden)
samfalligheterna.se##.td-cpt-post:has(a[href*="/sponsra"])
samfalligheterna.se##.td_block_wrap:has-text(Annons)
samnytt.se,samnytt.nu##a[href*="casino"], a[target="_blank"] img:not([class^="tweet-"]), a img[src^="/butik"]
samnytt.se,samnytt.nu##.sticky > div:has(img[src^="/butik"])
sanghafte.se##.widget_cooperations
sanghafte.se##.wp-show-posts-single:has(a[href*="casino"], a[href*="kasino"], a[href*="betting"])
sbf.se##.sv-cookie-consent-banner, .hiq-partners-banner
scanaktier.se###overlay-black
schack.se##.schac-widget
schoolido.se##.so-cookie__area
screen-marknaden.se##.fo-banner, .fp-banner
sdhl.se,ssl.se,storvretaibk.se##.rmss_module-block-linked_image, a[href*="svenskaspel.se"]
sdhl.se,ssl.se,storvretaibk.se,obosdamallsvenskan.se,elitettan.se,ifiske.se##.cc_banner-wrapper
selectAdvertiserElement$domain=bebisvarlden.se
senses.se##aside:has-text(Annonser:)
senses.se##a[href*="casino"], a[href*="spelsajt"], a[href*="betting"]
sexpacket.se##+js(aeld, /contextmenu|cut|copy|paste/)
sexpacket.se##.info_cookies
se.azrhymes.com##div[id^="azrhymes_com_between_content"]
shoegazing.se###main-sidebar .widget_media_image, #post-sidebar .widget_media_image, #content > .code-block
shortcut.se##div[class^="baner"], a[target="_blank"] img
shortcut.se##.category-tag:has-text(/annons/i):upward(.ArticleListItem)
sidebanner$image,domain=samnytt.se|samnytt.nu
signprint.se##.topbanner
signprint.se##p:has-text(SPONSR):upward(.elementor-widget-jet-listing-grid)
siljannews.se##article:has(a[href^="/annons"])
siljannews.se##a[target="_blank"]:upward(2)
siljannews.se##h3:has-text(/Annons/i) + div
siljannews.se##p > a:not([href*="siljannews.se"]):not([href^="/"]) img
siljanskok.se##a[target="_blank"][rel="nofollow"]:upward(1)
siljanskok.se###app > div[data-reactroot] > div:first-child:has(a[target])
sillyseason.se##li:has(a[href*=".se/odds/"], a[href*="/betting/"], a[href*="kasino"], a[href*="/promomen/"])
sillyseason.se##strong:has-text(casino):upward(li.sidebar-widget)
sillyseason.se###text-41, #leader-wrapper, a[href^="/till/"][target="_blank"]
siriusbandy.se,vetlandabk.se##[id$="-ad"]
si.se,sweden.se###cookie-manager
sjofartstidningen.se###newsletter-overlay, #newsletter-modal
sjofart.ax##section.huvudsektion:style(margin-top:unset!important)
sjofart.ax##:is(.sjofa-top-takeover, .sjofa-artikel-pano):upward(section)
sjostadsbladet.se##a.td_single_image_bg, span.td_single_image_bg[data-img-url*="Annons"]
sjostadsbladet.se##.td-category-pos-:has(a[href*="casino"])
skaneplus.se##div[style="padding-top:0px;padding-right:0px;padding-bottom:0px;padding-left:0px;flex-basis:50%"]:has(a:not([href*="skaneplus.se"]):not([href^="/"]) > img)
skanesport.se###black-studio-tinymce-3, .menu-item a[target="_blank"], .footer-widgets
skargarden.se##article:has([title^="Annons"], a[href*="/annons"])
skargarden.se###topbanner, #mittbanner, #topbannerm, #mittbannerm
skidspar.se###videoad
skillingaryd.nu,xn--vrnamo-bua.nu###more-banners
skk.se###cookie-button-banner, .campaigns, [id*="GlobalCampaigns"]
skogen.se##.jobslider.up
skogsforum.se##.masthead, .col-right, a[href^="https://goo.gl/"], a[href*="//bit.ly/"], a[target="_blank"][onclick], #ap1, .modal, .modal-backdrop
skogssallskapet.se,formas.se,rf.se##body:style(overflow:initial!important; position:initial!important;)
skogssallskapet.se,formas.se,rf.se##.env-modal-dialog--show, .env-modal-dialog__backdrop
skolfamiljen.se##.right-sidebar aside[id^="block"], .right-sidebar aside[id^="adguru"]
skolporten.se##.article-short:has(a[href*="/sponsrat-innehall"])
skrattnet.se##.region-sidebar-second
skrattsajten.com,norpan.se##.cookieScript
skrattsajten.com,norpan.se##+js(acs, $, e.preventDefault)
skyltat.se##.sidebar
skyscanner.se###modal-container, div[data-testid="advert-card-gam"]
smartsenior.se##.ss-modal, .modal-mobile-app
snowmobile.se##div[itemtype="https://schema.org/WPAdBlock"], .bs-wrap-gdpr-law
sokbat.se##a[target="_blank"][onclick]
sonicmagazine.com,ratsit.se,dagensinfrastruktur.se,nyaprojekt.se,nordiskaprojekt.se,svenskbyggtidning.se,grontsamhallsbyggande.se##[class^="ad-"]
so-rummet.se##h3:has-text(/annonser/i):upward(.view-nya-lankar-front)
so-rummet.se##.article-list:has(.sponsrad-over)
so-rummet.se##.block-rr
so-rummet.se##.link-list-item:has(img[src*="sponsrad"])
spanaren.se,horisontmagasin.se,shoegazing.se##.textwidget a[target*="blank"] img
spelagratis.se##.sidebar-right, .ad_header + p
spelhubben.se##html, .unselectable:style(-moz-user-select:initial!important; -webkit-user-select:initial!important; -webkit-touch-callout:initial!important; user-select:initial!important; -webkit-tap-highlight-color:initial!important; cursor:initial!important;)
spelhubben.se###slideout
spelhubben.se,husbilsplats.se##+js(acs, document.oncontextmenu)
spelochfilm.se##a[href*="casino"]:upward(.mh-posts-stacked-wrap)
spelochfilm.se##.mh-sidebar .textwidget
spelo.se,lokalguiden.se,svenskverkstad.se##.banner-container
sponsor$image,domain=obosdamallsvenskan.se|elitettan.se
sportal.se##.cookie-div, a[href$="/banner/"]
sportbilen.se###text-4
sportbladetplay.se##body.dimmed:style(overflow:unset!important)
sportbladetplay.se##.ui.page.dimmer:has(div[class^="CookieConsentPopup"])
sportbloggare.com##div.section-body-plus:has-text(/bonus|casino/i)
sportbloggare.com##.container:has-text(Senaste nyheterna om spelbolag:)
sportbloggare.com##.partners-box, .cube-bonus-list, .section-featured-links-column, .section-bonus-list, a[href="https://sportbloggare.com/casino-bonus"], a[href="https://sportbloggare.com/bettingsidor"], a[href="https://sportbloggare.com/betting-bonus"]
sportbloggare.com##.section-body-plus .body-block:has(a[href*="betting"])
sporthalsa.se##a[href*="/annonsering"]
sporthalsa.se##h4:has-text(veckans produkt):upward(3)
sporthalsa.se##.header_top, #media_image-2, #text-6, article[class*="veckans-produkt"]
sportlovin.se##.visible-xs, .visible-lg
sportpanelen.se##.textwidget:has(a[href*="casino"])
sportsnews.se,xn--sporthnt-5za.se###secondary:has(a[href*="casino"])
sporttv.nu##a[onclick*="bannerClick"], #linkus, .details-bet-banner
spray.se##body:style(-webkit-user-select: text !important; user-select: text !important;)
spray.se##section[class*="casino"], a[href*="casino"]
spray.se##+js(set, googletag, 1)
spray.se,vinochmatguiden.se##+js(set, window.WURFL, 1)
stallet.se##.pnlAdTop
stallet.se##+js(alert-buster)
startaochdriva.se##.banner-right, .banner-left, .wpb_single_image a[target="_blank"], .tdm-popup-modal-wrap
startaochdriva.se##:is(.latest-post, .td-cpt-post):has(a[href*="/sponsrat"])
stegforhalsa.se##[class*="jsx-"][style*="position: sticky"], .bc--grey-neutral-50[style^="min-height"]
stoppapressarna.se##.premium-page-ad, .footer-banner-wrapper, div[id^="stopp-"]
storyhouseegmont.se##body.freeze-scroll:remove-class(freeze-scroll)
storyhouseegmont.se##div[class^="Navigation__Overlay"]
streamio.com,nyan.ax,spelhubben.se,illvet.se,varldenshistoria.se##+js(aeld, contextmenu)
surfa.se##div[class*="-promo"], div[class*="prisjakt-"]
surfa.se,teknikfreak.se###loader-wrapper
svampguiden.com##.label-sponsor:upward(.panel)
svartgul.se##li.embedded
svartgul.se,eventeffect.se,executiveeffect.se,saleseffect.se###panorama
svd.se##article:has(div[class^="NativeBarWrapper"])
svd.se##body:style(visibility:visible!important;)
svd.se###mega-ad-wrapper, div[class*="advertory"], div[data-custom-ad-handled="true"], span[data-id="bottom-sticker-offer"], div[data-context-pageview*="native-svd"]
svd.se,chef.se,vvsforum.se,elinstallatoren.se,arkitekten.se,natursidan.se,svenskfarmaci.se,da.se,frisor.se##.Ad
svenskafans.com##.puff__ad-heading, ad-skyscraper__wrapper, iframe[title*="Bet 365"]
svenskahousegruppen.se##body.modal-open:style(overflow:initial!important)
svenskahousegruppen.se###eprivacyModal, .modal-backdrop
svenskalag.se##.cookie-overlay, .cookie-box
svenskarnaochinternet.se,internetstiftelsen.se###newsletter-sliding
svenskbyggtidning.se,nyhetersto.se,bussmagasinet.se,brollopsmagasinet.se,borattforum.se,globalpolitics.se,batliv.se,em-fotboll.se,elinor.se,fotbollsresultat.com,automation.se,vm-fotboll.se,husbyggaren.se,vildmarken.se,fisheco.se,nyhetsbyranjarva.se,it-finans.se,it-halsa.se,it-kanalen.se,it-pedagogen.se,it-retail.se,it-hallbarhet.se,battregolf.se,sporthalsa.se,revisionsvarlden.se##a.gofollow[data-track]
svenskelitfotboll.se##custom-ad, sponsors
svenskelitfotboll.se##.image-block:has(a[class*="sponsor"])
svenskfarmaci.se##.Dialog[data-dialog-skip-auto-open-for-utm-source-value="Newsletter"]
svenskfotboll.se##.news-multi-link--sponsor
svenskgolf.se##.highlight:has(.partnerLabel)
svenskgolf.se,husohem.se,tidningenhalsa.se,vagabond.se,praktisktbatagande.se,akaskidor.se,utemagasinet.se,sportfack.se##.partnerCard, .partnerContent, .entry-content figure.wp-block-image, .category-partner, .ams-playad-injected
svenskhistoria.se##.widget_et_ads, .module-etads, #text-13, #block-4, a[target="_blank"][rel="noopener noreferrer"], a > img[width="300"][height="250"], a > img[width="800"][height="175"], a[href*="casino"], a[href*="poker"], a[href*="kasino"], a img[width="1000"][height="300"]
svenskhistoria.se##.widget_text:has(a[href*="casino"])
svenskjakt.se###survey-dialog
svensktgolfforum.se##[data-ad-id], .darkenwrapper
svensktidskrift.se###bannercolumn, img[title^="Annons"]
svensktidskrift.se##.tf_svg_lazy:style(transition:none!important; filter:none!important; transform:none!important;)
svenskverkstad.se##app-exposure-small
svenskverkstad.se##svv-short-news-widget:has(.native-news-link)
svenskverkstad.se##svv-wide-news-widget:has(.annons)
sverigesindustri.se##.article-item:has(.article-label--sponsored, .article-item--sponsored)
sverigesnatur.org##div[id^="sverigesNaturPopup"]
sverigespringer.se##.cd-card-bar:has-text(/annons/i):upward(.cd-sidebar-item, .cd-news-card)
sverigespringer.se##.cd-desktop-banner
sverige.nu##a[href*="casino"]
sweclockers.com##div[class^="card-info"]:has-text(/spons/i):upward(.card)
sweclockers.com###prisjakt-popular, .ad:not(.adPanorama), .adForumSticker, .dark-mode__sponsor
sweclockers.com##.ad.adPanorama:style(height:100px!important; position:absolute!important;)
sweclockers.com##.bbSize:has-text(Sponsormeddelande):upward(.bbRelatedBox)
swedroid.se##a[target="_blank"]:upward(li.Notice):remove()
swedroid.se##div[id$="_ad"], div[id$="_ad_mobile"], .externalTopMobile, #externalTopMobile, .externalBottomMobile, a[href^="//www.prisjakt.nu/produkt"], #nativendo-mainfeed + aside > .article, .article-footer > h3, .article-footer > .aeChart, #newExternal
swedroid.se##span:has-text(/sponsr/i):upward(.article)
swedroid.se##+js(set, checkAdsBlocked, noopFunc)
swedroid.se##.mostReadMobile:has-text(/annons/i)
swedroid.se##.puff:has(script[src*="lwadm.com"])
swehockey.se##[class*="-reklam"], .sif-sponsorer, .teaserblock, .commonblock a:not([href^="/"], [href*="/swehockey.se"])
sydasien.se##.thb-cookie-bar
sydnarkenytt.se##.toppbanner-outer, .reklamplats_hspalt, .egenbanner
synonymer.se##+js(cookie-remover, /^ev_did|ev_sid/)
synonymer.se##.create-account-banner, .buy-premium-banner, div[class*="pb-"] > div.text-center
tabyallehanda.se##p:has-text(ANNONS)
tabyallehanda.se##section[id^="Panorama"]
tandlakartidningen.se##[class^="ad-container"], [class^="adbox-single"], div[id^="takeover-"]
tasteline.com##.article.related > a[href*="&utm"][target="_blank"]
tasteline.com##.popup-overlay
tasteline.com##.popup:style(overflow: auto !important;)
techmag.se##div[style="clear:both;float:left;width:100%;margin:0 0 20px 0;"]:has(.contentadx)
techmag.se##.popup-overlay, div[id^="techmag_com"], .contentadx
techmag.se##.widget_codewidget:has(div[id^="techmag_com"])
teknifik.se##.post:has(.sponsor)
teknikguiden.se##:is(.vce-sticky, .vce-content-bottom):has(a[target])
tekniknytt.se##.label:has-text(/samarbete|annons|reklam|presenteras av/i):upward(a)
tekniknytt.se##:is(.article_widget_preview, .article_widget_listing):has(a[href*="casino"], a[href*="kasino"])
tekniknytt.se##:is(.top-news, .big_article):has(img[src*="casino"], img[src*="surfeo"])
tekniknytt.se##[onclick^="ga("]:remove-attr(onclick)
tekniksmart.se##center:has-text(/annons/i):upward(1)
tekniksmart.se##.code-block, main > div:last-child:not(:only-child), #uid_08313ba73, #uid_ab3738b5a, .jeg_header_wrapper .jeg_midbar
tekniksmart.se##.wpb_row:has(a[href*="casino"])
teknikveckan.se##.pill:has-text(/spons/i):upward(.grid-item, .pinned, .articleFlow-item)
teknikveckan.se,di.se,dn.se,skillingaryd.nu,xn--vrnamo-bua.nu,vardfokus.se,kamerabild.se,tripadvisor.se,swedroid.se,bettingstugan.se,expressen.se,dagensopinion.se,driva-eget.se,bioenergitidningen.se,ifokus.se,padelfeber.se,sv.picmix.com,ifragasatt.se,ehandel.se,jaktojagare.se,sportbloggare.com,bovision.se,familjeliv.se,tidningenridsport.se,golflivet.se,vemringde.se,brollopstorget.se,fastighetsvarlden.se,borskollen.se,aktiespararna.se,receptfavoriter.se,tyda.se,mittforetag.com##.ad
teknologiexperten.se##a:has(img[src*=".se-www"]), a[href*="casino"]
temaarkiv.se##.md\:mt-\[100px\]:has(script[data-adfscript])
temadagar.se##+js(acs, chp_adblock_browser)
temadagar.se##.ez-sidebar-wall
temperatur.nu##.holidAds:upward(1)
tennisportalen.se##h4:has-text(/spons/i):upward(.td-pb-row [class*="td-pb-span"])
testfakta.se##.row-uppdragstest
thatsup.se##+js(set, canShowAds, true)
thelocal.se##.ad-container-section, .article-sponsored, div[data-hasbanner="yes"]
thelocal.se##.ra-widget-article-tag:has-text(/partner/i):upward(.ra-widget-panel)
thelocal.se##.single-article-related.single-article-related-short:style(height:unset!important; overflow:unset!important;)
thelocal.se##.single-article-related.single-article-related-short::after:style(background:unset!important;)
thepattayanews.se##a.td_single_image_bg:not([href*="thepattayanews.se"]), #tnp-modal
thorengruppen.se,utslappsratt.se,heleneholmsif.se,trafikskola.se,melodifestivalklubben.se,morotsliv.com##+js(set, em_track_user, false)
thorengruppen.se,utslappsratt.se,heleneholmsif.se,trafikskola.se,melodifestivalklubben.se,morotsliv.com##+js(set, exactmetrics_frontend, undefined)
tidningenbalans.se##div[style*="z-index: 999; background-color: rgba(0, 0, 0, 0.5)"], .bg-grey.hideOnPrint, .bg-adYellow
tidningenbalans.se##p:has-text(/i annonssamarbete med/i):upward(.flex.overflow-hidden)
tidningendacksnack.se##.ann-puff
tidningenglobal.se,tidningensyre.se,landetsfria.nu,fempers.se##.revive-box
tidningennara.se,odenochaventyr.se##.cookie-bar
tidningenridsport.se##body:remove-class(cli-barmodal-open)
tidningenridsport.se##.entry-content:style(display: initial !important;)
tidningenridsport.se##.subscribe_now_popup, .type-native, #captive, .hldr_takeover_nl.show, .hldr_takeover
tidningenskriva.se##section.widget_text:has(div[id^="ad-"])
tidningen.djurskyddet.se##.ai-track
tidningen.nu##span:has-text(/^Annons$/):upward(1) + .textwidget
tidningen.se##.sidebar .widget_widget_code, .casino
tillnyktrad.se,webhallen.com##.cookie-consent
tittapavideon.se##.adv
tlnt.se##div[id^="ad-block"]
tlnt.se##.fakta-list:has-text(/annons/i)
tonyhatefnejad.se,lyckasmedbakning.nu,pinkprogramming.se,brl.se,naturnaraskogsbruk.se##.preloader
totallyorebro.se,totallystockholm.se##div.tot-content-preview-container-small[style*="border-top:4px solid #ffb200;"], .content-overlay--black, a[href*="casino"], a[href*="/sponsrat/"], a[href*="/sponsrat/"] + p.tot-content-preview--meta, .newaddiv, .tot-sidebar
totallyorebro.se,totallystockholm.se##[class*="tot-content-preview-container"]:has(a[href*="casino"], a[href*="kasino"], a[href*="betting"], a[href*="spel"]):remove()
trafikradion.com##.right
tranakampsport.se##.w-dyn-item:has(.sponsrad-artikel-wrapper:not(.w-condition-invisible))
traning40plus.se##[id^="bunyad"]
travelnews.se##.bottom-bar--animate-in, #job_ads_scroller, .header_banner
travnet.se##.hidden:has(div[id^="travnet_"])
travronden.se##a[href*="/sponsrat/"]
travronden.se##div:matches-css(visibility: hidden):has-text(ANNONS)
travsport.se,gavletravet.se##.banner-component, .partners, .cookie-meddelande
trendenser.se##strong:has-text(/reklam/i):upward(.post_feed_post)
trendenser.se##.featured-post:has(a[href*="/category/reklam"], a[href*="/category/annons"])
trendenser.se##.post_feed_post:has(.sponsor-info)
tripadvisor.se##a:has-text(/Sponsrat av|i samarbete med/i)
tripadvisor.se##[class$="banner_ad"]
turismnytt.se##.site-wrap > .row > .col-sm-3
turistmal.se###col_right
tv4play.se,tv4.se,fotbollskanalen.se,koket.se##button:has-text(Besök annonsör)
tv4play.se,tv4.se,fotbollskanalen.se,koket.se##+js(json-prune-fetch-response, playbackItem.isStitched, , propsToMatch, url:a2d.tv/play)
tv4play.se,tv4.se,fotbollskanalen.se,koket.se##+js(xml-prune, Ad, , /fwmrm.net\/ad\/g/)
tv4play.se,tv4.se,fotbollskanalen.se,koket.se##.avod-web-player-pause:style(background-color:transparent!important;)
tv4.se##.maxetise
tv24.se##li[id^="infeed"]
tvmatchen.nu##.bet365, .panorama-wrapper, .tvg-manager-box, .tv102945, .tv102987, #event_banner, .go-to-partner, .odds, #text-13
tvprogram.se##.backdrop, .fcb
tv.nu##a[href*="adform.net"], .ad-fullscreenWallpaper__container
tv.nu##body:remove-class(takeover-loading)
tv.nu###tv-schedule section:has-text(ANNONS)
tyda.se##.frontpage_article:has(a[href*="casino"], a[href*="kasino"], a[href*="betting"], img[data-cfsrc*="Sponsra"])
typkanske.se##.adbar
underbaraclaras.se##.jet-listing-dynamic-field__content:has-text(/annonssamarbete|reklamsamarbete/i):upward(.jet-listing-grid__item)
undertian.com###cookieNotification, .gad, div[style^="font-size:11px; margin-left"], div[style^="font-size:11px; margin-left"] + div[style]
undervarttak.se##.middle-banner
ungdomsfotboll.se##div[id^="ungdo-"]
universitetslararen.se##div[id^="unive-"]
upphandling24.se##aside .textwidget:has-text(ANNONS)
upphandling24.se##.type-partnerartikel
uppsalanyheter.se###banner-top-block
uppsatser.se##.results li[style^="margin"]:not(.result)
upptack-sverige.se##.front-cta:has-text(/sponsrat innehåll/i)
usabil.nu##.image-post-link[target]
utm_$document,removeparam=/^utm_/,domain=tv.nu|booli.se|expressen.se|aftonbladet.se|bostad.blocket.se|dagensps.se|prisjakt.nu|vinborsen.se
utsidan.se##.clamzone
utsidan.se##.betart-marker:matches-css(after, content: /Annons/i):upward(.documentpush-group)
vackertvader.se##div[class^="ad-300x250"], div[class^="ad_300x250"]
vackertvader.se,tidningenskriva.se,veckansnyheter.se,eventeffect.se,executiveeffect.se,saleseffect.se##.cc-window
vadvivet.se##html.has-intro-popup:remove-class(has-intro-popup)
vadvivet.se##html.show-intro-popup:remove-class(show-intro-popup)
vadvivet.se##.intro-popup
vagabond.se##.latest-article-native
varden.se##app-native-puff, .header-top-banners
varden.se##.carousel-slide:has(.sponsored-label)
vardfokus.se,tidningenridsport.se##.cli-modal-backdrop
vardpraktikan.se###nyhetsbrev
varldenshaftigaste.se##[id*="annons"], #getFixed
varmepumpsforum.com##.stopjump
varmepumpsforum.com##a[target]:upward(.frontlinks tr)
varmepumpsforum.com,poolforum.se,lindenytt.com,autopower.se,arjeplognytt.se,jaktsidan.se##a[target="_blank"] img[alt]
vartgoteborg.se##div[class^="Popup"], div[class^="CookieBanner"]
varvat.se##.wpb_single_image a[target], .gp-footer-2
vasterastidning.se##article[data-section="nativeannons"]
vasterastidning.se##.row:has(a[href*="casino.se"])
vasterastidning.se##:is(h2, h5, .kicker):has-text(ANNONS):upward(article, div.row)
veckansmiddag.com###load
veckorevyn.com##.annons-block
veckorevyn.com##.g1-mosaic-item:has(.category-annonssamarbete)
veterinarmagazinet.se##.nyhet-ad
vf.se,hjotidning.se,kt.se,kt-kuriren.se,sla.se,mariestadstidningen.se,filipstadstidning.se,fryksdalsbygden.se,nwt.se,arvikanyheter.se,nkp.se,saffletidningen.se,provinstidningen.se,dalslanningen.se,nlt.se,skaraborgsbygden.se##[data-testid="ad-area"], footer + div.shadow-lg.fixed
vibilagare.se##a[href^="/partnermaterial/"]
viivilla.se###rich-media-wrapper
viivilla.se##.teaser:has(.teaser__native-marker)
vilaser.se##.Internal-ad
villalivet.se##.mtsnb, .villalivet-target, a[href*="/sponsrat-innehall/"], div[data-td-block-uid="tdi_85"], a[href*="utm_campaign"][target="_blank"], div[data-td-block-uid="tdi_87"]
villalivet.se##:is(a, span):has-text(/sponsr/i):upward(3)
villatidningen.se##.wppsac-post-carousel:has(a[href*="/spons"])
vimedbarn.se##button:has-text(/annons/i):upward(.owl-item):remove()
vimedbarn.se##.annonsinlagg, .annonsen
vinbanken.se##.fancybox-lock:style(overflow-y: auto !important;)
vinbanken.se##.push-to-newsletter, .fancybox-overlay
vinbanken.se##.top-add, .sidebar-adds, .spons-content
vinliv.se##.product_banner_wrapper
vinochmatguiden.se##.popup_missa-inget
viseniorer.se##.topheaderinfo
viseniorer.se##.leftinfo:has-text(/Externa artiklar:|Länktips:/)
vi.se##body.cookie-modal-open:style(overflow:unset!important;)
vi.se###westander-cookie-dialog, .Cookie-consent__backdrop
vk.se,folkbladet.nu,nordsverige.se,mellanbygden.nu,vasterbottningen.se,lokaltidningen.nu##.vkmui-Text--grey, [class^="adContainer"], div[class^="bordersAndShadows"] > div[style^="min-height"]:only-child, div[data-track-id="family.Familjeannonser"], div[class*="adElement"]
vmj.se##.sidebox:has-text(/Externa länkar|Artiklar/)
vmj.se,danskaspraket.se,digitalavykort.se##.topdiv
vmj.se,danskaspraket.se,digitalavykort.se,viseniorer.se##.cc-cookies
vm-fotboll.se##a[href*="/go/"][target], .category-kampanjer
vm-fotboll.se##.fusion-text:has-text(Online casino)
voister.se##div[class^="articles_articleBrief"]:has(div[class*="articles_campaign"])
voodoofilm.org##.card-header:has-text(Annons):upward(.card)
voodoofilm.org##.content-news:has(span[id*="Sponsored"])
voodoofilm.org##.page-panorama
vovve.net##span:has-text(/^i samarbete med/i):upward(2)
vovve.net###sticky_ad, div[style*="ad_hor.gif"], a[href*="casino"], a[href*="kasyno"], a[href*="betting"], a[href*="spelsajter.eu"], a[href*="spelsidor.org"], a[href*="oddsgurun.com"], a[href*="betsidor"], a[href*="välkomstbonusar"]
webbjobb.io##.cookie
webbkameror.se###cookiescript_injected
webbkryss.nu##.skyad-wrapper
webb-tv.nu##[id^="adservice"]
webhallen.com##.takeover-link
whowhatwear.co.uk#@#a[href*="/click.linksynergy"] img
www.aftonbladet.se##+js(nostif, TAKEOVER)
www.expressen.se##+js(set, detect, noopFunc)
www.expressen.se##.video-player:remove-attr(data-ad-config)
www.expressen.se,di.se##+js(aeld, contextmenu, .disabled)
xn--lnforum-exa.se##.LFRBox
yogafordig.nu##.popup-large, .popup-bottom, .square-banner-wrapper
ysektionen.se##.yweb-news-paper-banner
zeinaskitchen.se,trafiksakerhet.se,boktugg.se,lakartidningen.se,villalivet.se,matsafari.nu,forexgruppen.se,fastighetsvarlden.se##+js(acs, monsterinsights_frontend)
zeinaskitchen.se,trafiksakerhet.se,boktugg.se,lakartidningen.se,villalivet.se,matsafari.nu,forexgruppen.se,fastighetsvarlden.se##+js(set, mi_track_user, false)
zeromagazine.nu##div[id^="ads"]
##.lazyb.panorama
##adsaga-banner
##article.NativeTeaser
##article.annons
##article.sponsrad
##article.article-list-item--sponsored-post
##article.article-sponsored
##article.article--sponsored
##article.category-partnerartikel
##article.category-promotion
##article.category-reklam
##article.category-samarbete
##article.category-samarbete-sponsrat
##article.category-samarbete-sponsrat-inlagg
##article.sponsrat-inlagg
##article.tag-adtraction
##article.tag-annons
##article.type-partnerartikel
##article[data-section="sponsrad"]
##aside.ad-container
##a#top-banner.banner-holder
##a.adv-link
##a.card.-sponsored
##a.is-native-ad
##a[data-bid="1"][href*="/linkout"]
##a[href$=".se/go/betsafe"]
##a[href*="casinopro.se"][target="_blank"]
##a[href*="cyberbetpromo.net/click"][target="_blank"]
##a[href*="doktor-se.onelink.me"]
##a[href*="tradedoubler.com/click?"]
##a[href*="utm_content=banner"] img
##a[href*="www.bildelaronline24.se"][target="_blank"]
##a[href*="www.reservdelar24.se"][target="_blank"]
##a[href*="/annonsartiklar/"]
##a[href*="/banner/klick/"] img
##a[href*="/click.adrecord"] img
##a[href*="/click.linksynergy"] img
##a[href*="/cvasino.se/"] img
##a[href*="/delivery.adnuntius.com"]
##a[href^="https://www.adsettings.com/scripts/reg_click."]
##a[href^="/banner/click/"] img
##a[id^="adBanner"][target="_blank"]
##a[onclick*="AdRotatePro"]
##a[onclick*="artikelbanner"]
##a[title="LeoVegas"]
##body[data-site-namespace="tailsweep"] #premiumAdWrapper
##div.NativeAd
##div.adDivLeft
##div.adDivRight
##div.adLinkInner
##div.adSidebar
##div.ad.container
##div.ad.panorama
##div.annonsbox
##div.bbPrisjakt
##div.holidAds
##div.outsideAdsWrapper
##div.panoramaAd
##div.toppannons
##div.wppasrotate
##div#ads-panorama
##div#ads_column
##div#ad_global_below_navbar
##div#annons_topp
##div#banner_right
##div#block-adreviveheader
##div#custom_ads_wrapper
##div#facebook-popup
##div#mega-ad-content
##div#outerAd
##div#outside-ads
##div#panoramaad
##div#panorama_ad
##div#reklam
##div#rich-media-ads
##div#schibsted-data-controller-sticky
##div#snow-container[style*="z-index: 999999"]
##div#toppannons
##div#topreklam
##div#zox-lead-bot
##div.CMACG_AdChangerWidget
##div.Container--ad
##div.External-ad
##div.adform-container
##div.adnuntius-ad
##div.ads-sticky-container
##div.adtech_slot
##div.advads-background
##div.ad-after-header
##div.ad-after-post
##div.ad-component
##div.ad-container-lg
##div.ad-panorama_dynamic-wrapper
##div.ad-toppbanner
##div.after-article-ad
##div.annons-yta
##div.article-ad-container
##div.ashe-preloader-wrap
##div.bam-ad-wrapper
##div.banner-size.proad
##div.before-article-ad
##div.better-ads-listitemad
##div.big-desktop-ads
##div.block-bean-header-banner
##div.borka-ad
##div.box--squareAd
##div.brix-ads-by-posttype
##div.bsa_pro_ajax_load
##div.column-article.tag-annons
##div.comment-ad_wrapper
##div.content-center-ad
##div.content_ad_top
##div.elementor-widget-wp-widget-adrotate_widgets
##div.elementor-widget-wp-widget-advads_ad_widget
##div.feed_ad
##div.fs-holid-live-widescreen
##div.helsida-ad
##div.inner_advertisement
##div.in-post-ad-wrap
##div.jeg_ad
##div.js-top-banner-container
##div.landscape-ad-space
##div.leeads-wrapper-desktop
##div.link-ads
##div.l-footer__adtext
##div.maaw-ad-slots
##div.medium-ad
##div.mgp-ads
##div.mosaico-ad
##div.navbar-ad-section
##div.novashare-buttons
##div.o-indenter--ad
##div.panorama-ad
##div.panorama-ad-standard
##div.partnership-ads
##div.phpbb-ads-center
##div.prebid-ad-slot
##div.sb-egmont-plugin
##div.schibsted-info-sticky
##div.sch-datacontroller--footer
##div.sch-datacontroller--subheader
##div.sgm-ad
##div.sgm-header-start-ad
##div.sgm-large-ad
##div.sidebar-annons
##div.sidebar-item .banner-box
##div.strossle-widget
##div.td-a-rec img
##div.td-banner-bg
##div.topmost-banner
##div.view-annons-banner
##div.vue-ad-wrapper
##div.widget_widget_dfp
##div[class$="popup-and-layer-ads"]
##div[class*="ai-viewport"][data-insertion-position]
##div[class*="bsaProContainer"]
##div[class^="borka-insider"]
##div[class^="borka-panorama"]
##div[class^="borka-widescreen"]
##div[class^="holid_desktop"]
##div[data-losjs^="borka-insider"]
##div[data-losjs^="borka-panorama"]
##div[data-losjs^="borka-widescreen"]
##div[id^="ad_insider"]
##div[id^="borka-insider"]
##div[id^="borka-panorama"]
##div[id^="borka-widescreen"]
##div[id^="matchads-"]
##footer .sponsors-area
##iframe#compricer_iframe
##img[alt="Leovegas"]
##img[alt="Spela på Betsson"]
##img[src*="/track.adtraction"]
##ins[data-revive-zoneid]
##td#reklam
##ul.adsmodern
###RightOuterBannerDiv
###advisa-iframe
###ad-fullscreen:not(body):not(html)
###ad-mega-container:not(body):not(html)
###ad-wallpaper:not(body):not(html)
###ad_topScroller:not(body):not(html)
###annons_head
###bottomAnnonsBar
###div-leeadsFullpageAd
###leeads-panorama-container
###strossle-below-article-thumbnails
###topBannerAds
##.Teaser--nativeAd:not(body):not(html)
##.adContainer:not(body):not(html)
##.adrotate-group:not(body):not(html)
##.adtoma_container:not(body):not(html)
##.adtrue-holder:not(body):not(html)
##.ad-rotator:not(body):not(html)
##.ad-single-news:not(body):not(html)
##.ad_container_bottom:not(body):not(html)
##.annonseArticle:not(body):not(html)
##.annons_mitten:not(body):not(html)
##.annons_panorama:not(body):not(html)
##.bannerclick:not(body):not(html)
##.b-ad__wrapper:not(body):not(html)
##.carrie-ad-block:not(body):not(html)
##.casino-ad:not(body):not(html)
##.category-annonssamarbete:not(body):not(html)
##.category-annons:not(body):not(html)
##.category-om-samarbeten:not(body):not(html)
##.category-samarbeten:not(body):not(html)
##.category-sponsrade-inlagg:not(body):not(html)
##.category-sponsrade-reklaminlagg:not(body):not(html)
##.category-sponsrad-artikel:not(body):not(html)
##.category-sponsrad:not(body):not(html)
##.category-sponsrat-content:not(body):not(html)
##.category-sponsrat-inlagg:not(body):not(html)
##.category-sponsrat-innehall:not(body):not(html)
##.category-sponsrat:not(body):not(html)
##.component-matchAds:not(body):not(html)
##.component-matchAds__content:not(body):not(html)
##.c-ad-wrapper:not(body):not(html)
##.c-ad__floating:not(body):not(html)
##.c-dfp_ads:not(body):not(html)
##.c-post--native-ad:not(body):not(html)
##.dfp-ad-widget-class:not(body):not(html)
##.dj-ad-size:not(body):not(html)
##.esmg-hb-slot:not(body):not(html)
##.favethemes-content-ad-bottom:not(body):not(html)
##.favethemes-content-ad-inline:not(body):not(html)
##.favethemes-content-ad-top:not(body):not(html)
##.footer-ad-wrap:not(body):not(html)
##.layerAdContainer:not(body):not(html)
##.leeads-advert:not(body):not(html)
##.loop-mobile-leeads:not(body):not(html)
##.mittenannons:not(body):not(html)
##.node-sponsored-article:not(body):not(html)
##.nyhet_wrapper_annons:not(body):not(html)
##.o-grid__ad-column:not(body):not(html)
##.penci-adsense-below-slider:not(body):not(html)
##.penci-infeed-fullwidth-ads:not(body):not(html)
##.plista_widget_outstream:not(body):not(html)
##.react-ad:not(body):not(html)
##.rmss_main-ad:not(body):not(html)
##.sponsorBanner:not(body):not(html)
##.sponsrad-artikel:not(body):not(html)
##.swp-ad-strossle:not(body):not(html)
##.sw-popular__article--ad:not(body):not(html)
##.sw-sponsored_post:not(body):not(html)
##.sw-tag-sponsored_post:not(body):not(html)
##.tag-sponsrat-inlagg:not(body):not(html)
##.teaser--native-ad:not(body):not(html)
##.thb_ad_header:not(body):not(html)
##.toppannonser:not(body):not(html)
##.widget_adonnews:not(body):not(html)
##.widget_ev_ad_widget:not(body):not(html)
##.widget_ic_ad_widget:not(body):not(html)
##._ning_outer._ning_jss_zone:not(body):not(html)
##[class*="advads_ad_widget"]:not(body):not(html)
##[id^="adace_ads"]
&autoplay$frame,removeparam=autoplay,domain=di.se|expressen.se
*$ping,domain=fiskejournalen.se
-popup-analytics
-tracking.js$domain=aftonbladet.se|godare.se|livsstil.se|svd.se
/468adrotate.php
/Advertisement$image,domain=sportbloggare.com
/Ad/*$domain=hallbyhandboll.se|skiljebosk.nu
/AffiliateHelper$domain=allas.se|elle.se|femina.se|hant.se|mabra.com|residencemagazine.se|svenskdam.se|motherhood.se
/AiMatch$script,domain=morningstar.se
/AnnonsClickScript.js
/Annons$domain=internetlankar.se
/AudienceTarget$script,domain=morningstar.se
/Banners/webbannons
/BlogPortal/view/Statistics
/CookieBar$script,domain=morningstar.se
/DO-theme/ads.js
/DynamicGAFunctions$script,domain=morningstar.se
/EAS_tag$script
/EUModalDialog$script,domain=morningstar.se
/GA_EEC$domain=osterbottenstidning.fi|sydin.fi|vasabladet.fi
/Global/Annons/*
/Grejer.js$domain=dagensvimmerby.se|dagensvastervik.se|dagenskalmar.nu|dagenshultsfred.se
/HSSAnalyticsUtils.js
/Jofab_Blog/js/ads.min.js
/LoadSlotLocator.$script
/LogRocket.min.js$third-party,domain=~dsc.gg
/OneSignalSDKWorker$script
/Portalannonser/*$image
/QA.js$domain=qruiser.com
/QXA.$script,domain=qx.se|qruiser.com
/Scripts/ads/*$domain=osterbottenstidning.fi|sydin.fi|vasabladet.fi
/Scripts/burt/*
/Script/Ads.js$domain=dagensvimmerby.se|dagensvastervik.se|dagenskalmar.nu|dagenshultsfred.se
/SitesterSurvey*.$script
/Smile_ElasticsuiteTracker/*$script
/SponsorsList$script,domain=hockeyallsvenskan.se
/TSPD/*$script,domain=corren.se|folkbladet.se|mvt.se|nt.se|vt.se|vimmerbytidning.se|kuriren.nu|nsd.se|norran.se|pt.se|ekuriren.se|strengnastidning.se|kkuriren.se|sn.se|eposten.se|unt.se|helagotland.se|kindaposten.se|gotlandjustnu.se
/TopBanner$subdocument,domain=hitta.se
/TrackPageView$domain=mestmotor.se
/Vizzit/vizzit.$script
/Web%20Analytics/*$script
/ab_appnexus_ads
/ab_stats_params$domain=aftonbladet.se|skonhetsredaktorerna.se
/ab_tracking$domain=aftonbladet.se
/adReloader$domain=morningstar.se
/add-ads.js$domain=fria.nu|stockholmsfria.se
/add-page-view$domain=cykla.se
/adform.js$domain=bohuslaningen.se|stromstadstidning.se|markposten.se|harrydaposten.se|partilletidning.se|sttidningen.se|molndalsposten.se|kungalvsposten.se|kungsbackaposten.se|alingsastidning.se|ttela.se|gp.se|hallandsposten.se|hn.se|mellerudsnyheter.se
/adnami/macro$script
/adnuntius_top_scroll
/adn/adn-setup.$script
/adobe/se/target-main-at.js
/adpage$domain=hotellorestaurang.se|byggfakta.today|citymark.today
/ads.article.js
/adsense.index.js$domain=husvagn.se|husbil.se
/ads-countdown.js$domain=aftonbladet.se|livsstil.se|godare.se
/ads-dm.js
/ads.for.me/jsa?$script
/ads.js$domain=flashback.org|onkologiisverige.se
/ads/adnami-conf.js
/ads/global-conf.js
/ads/load-dm.js
/ads?$domain=cirkulation.se
/adtracker$domain=beernews.se
/advertisement-dfp$script
/ad-render$domain=internetmedicin.se
/ad-takeover
/ad-widget
/ad-$image,domain=schack.se
/ad.aspx?
/ad/getNouw.$script
/ad?platform$domain=viaplayradio.se
/ad_acknowledgment$xmlhttprequest
/ad_in_article$script,domain=affarsvarlden.se
/affiliategallery$domain=allas.se|elle.se|femina.se|hant.se|mabra.com|residencemagazine.se|svenskdam.se|motherhood.se
/aftonbladet/crypt/?lpkey$all
/ajax-hit-reg.php?
/ajax/ads.php$domain=garaget.org
/ajax/docu_stats.jsp
/aller-ads
/amplitude$domain=mytaste.se
/analytics$domain=gbgfotboll.se|stff.se|svenskfotboll.se|di.se|etc.se|vackertvader.se|skogsforum.se|skolporten.se
/analytics-bmb
/analytics/cts.min.js
/analytics/gallup
/angry-golick-$script
/annonsbanners
/annonslinje_
/annonssamarbete$xmlhttprequest
/annons$image,domain=dagensvimmerby.se|dagensvastervik.se|dagenskalmar.nu|dagenshultsfred.se
/annons-banner
/annons.aspx?
/annons/banner
/annons_hor.
/annons_ver.
/antiblock$domain=vmj.se|viseniorer.se|danskaspraket.se|digitalavykort.se
/apester-javascript-sdk.min.js
/api/a/b$domain=borskollen.se
/api/log$domain=bohuslaningen.se|stromstadstidning.se|markposten.se|harrydaposten.se|partilletidning.se|sttidningen.se|molndalsposten.se|kungalvsposten.se|kungsbackaposten.se|alingsastidning.se|ttela.se|gp.se|hallandsposten.se|hn.se|mellerudsnyheter.se
/api/natives?$domain=aktuellhallbarhet.se|byggindustrin.se|dagensmedia.se|dagensmedicin.se|fastighetsnytt.se|resume.se|dagenssamhalle.se|market.se|dagligvarunytt.se|privataaffarer.se
/api/sponsors$domain=aikhockey.se|almtuna.com|bikkarlskoga.se|bjorkloven.com|brynas.se|difhockey.se|frolundahockey.com|farjestadbk.se|hockeyallsvenskan.se|hv71.se|ikoskarshamn.se|kalmarhockey.com|leksandsif.se|lhc.eu|luleahockey.se|malmoredhawks.com|modohockey.se|moraik.se|nybrovikings.com|orebrohockey.se|roglebk.se|shl.se|skellefteaaik.se|sodertaljesk.se|taif.nu|timraik.se|vaxjolakers.se|vikhockey.se|vik.se|ostersundik.com
/api/s/track$xhr,domain=eniro.se
/api/tracker?$image
/appinsights/*/track
/appnexus$script
/app.php/adsview$xmlhttprequest
/article-analytics$domain=bulletin.nu
/artikelannons/*
/artiklar/partner$xhr,domain=mestmotor.se
/arto/api/event$domain=arkitekten.se|natursidan.se|svenskfarmaci.se
/assets/DynamicAds-
/assets/js/ads.js$domain=dagensopinion.se
/assets/partnerstat.php?partner=$xmlhttprequest
/assets/site/modules/GTM_
/assets/site/modules/ctm-
/assets/tracking$domain=hornbach.se
/assets/yb_$domain=vackertvader.se
/ast.$script,domain=blocket.se
/atomic-blocks$script,domain=foretagsverige.se|forskningsverige.se|motorbibeln.se|hallbarhetsverige.se|tillvaxtsverige.se|grillbibeln.se|kampenmotcancer.se|folkhalsasverige.se
/atoms/images/*banner$domain=etc.se
/at_banners$domain=alandstidningen.ax
/a?callback=pfmod.saveadsettings
/bannersidor/*
/banners$domain=magasinetparagraf.se|sporttv.nu|cykla.se|vatternrundan.se|dagenstv.com|sydkusten.es|pellesoft.se|dykarna.nu|varmepumpsforum.com|poolforum.se
/banners/annons
/banners/scripts/adx.js
/banners/*casino$image
/banner$domain=revisionsvarlden.se
/banner$domain=thepattayanews.se
/banner/ads/*
/banner?cg$xhr,domain=blocket.se
/betald-exponering$image
/bigdatapushworker.js$domain=eurocampings.se
/bilder-for-annonser$image
/bilder/ads/*
/bilder/annonser/*
/bilder/annons$domain=webbkameror.se
/bilder/betalannonser
/bilder/logotyper/partners
/bilder/sponsorer
/bitcsys/js/bit.js
/block/samarbetspartners$image
/bloggerfy/tracker
/blogpoststatistic/impression
/blogpoststatistic/view
/blogs/log_pageview
/bmbBurt.$script
/bmbDfpUtils.$script
/bmbFusionUtils.$script
/bmb-related-teasers$xmlhttprequest
/bmb/*/native/boosted$xmlhttprequest
/bnrimg$domain=nordiskskog.se
/bnrscr?$domain=motormagasinet.se|food-supply.se|dagenshandel.se|plastnet.se|habit.se|woodnet.se|foodnet.se|transportnet.se|processnet.se|packnet.se|verkstaderna.se|medtechmagazine.se|recyclingnet.se|rt-forum.se|uochd.se|lifesciencesweden.se|fri-kopenskap.se|cleannet.se|framtidensbygg.se|entreprenad.com|metal-supply.se
/brand-metrics$domain=hemnet.se
/bundles/comscore$domain=expressen.se
/bundles/exp-analytics$domain=expressen.se
/bundles/ga-$script,domain=expressen.se
/bundles/parsely$domain=expressen.se
/bunsen/events$domain=yelp.se
/burst-statistics
/casinokollen$all,domain=aftonbladet.se
/casino_utan_licens$image
/cdigo-audit.js
/cecado/advisible.js
/census.js?bust=release
/clickperformance$domain=radio.se
/clicktracking.siteseeker
/closest-native$domain=expressen.se
/cmpv2$domain=m3.se|pcforalla.se|macworld.se
/cmp.js$domain=praktisktbatagande.se|hemtrevligt.se|vagabond.se|tidningenhalsa.se|utemagasinet.se|svenskgolf.se|mestmotor.se|sportfack.se|husohem.se|minhast.se|kalleanka.se|halge.se|bamse.se|akaskidor.se|husvagnochcamping.se|classicmotor.se|scandinavianretro.com
/cm-ad-changer-server
/collect?v$domain=thelocal.se
/content_images/*casino$image,domain=ng.se
/conversions/tracking.js$third-party
/cookieconsent$script,domain=akademiskahus.se|lundagard.se|fuska.nu|kiacarclub.se|nyheteridag.se|internetstart.se|svampguiden.com|scanaktier.se|obosdamallsvenskan.se|elitettan.se|bike.se|runnersworld.se|offside.org
/cookiesCon.js$domain=sydnarkenytt.se
/cookiespolicynotificationbar$domain=svenskahousegruppen.se
/cookies-and-content-security-policy$script,domain=cannabisifokus.se|futsalmagasinet.se|sd.se
/cookie-banner$script,domain=sprintchallenge.se|halsafitness.se
/cookie-consent$script,domain=minhembio.com
/cookie.min.js$domain=assistanskoll.se
/cookie_consent.js$domain=djungeltrumman.se
/cookie_policy.js$domain=nasdaqomxnordic.com
/cookie_popup$script,domain=trafikradion.com|trafik24.se
/cpg_ads.$script
/cs1pc.js$domain=kiaindex.se
/ctr-prd.cbs-measurements.
/cts.js$domain=allas.se|elle.se|femina.se|hant.se|mabra.com|residencemagazine.se|svenskdam.se|motherhood.se
/cx-emediate-userprofile-se
/data/banner$domain=nyaboendet.se
/data/track$domain=nyaboendet.se
/detroitchicago$domain=temadagar.se|svenskaorduttryck.se
/detroitchicago/cmbdv2.js$domain=wernamaten.se
/detroitchicago/denver.js$domain=wernamaten.se
/detroitchicago/*.gif?$image
/dh-adscale$domain=dh.se
/dh-adsticky$domain=dh.se
/dh-voldemort$domain=dh.se
/dialog$script,domain=marknadschefer.se
/discourse-adplugin
/discourse-prisjakt
/discourse-revive
/docunet_stats.js
/dovas/ads/*
/downloads.mailchimp.com/js/signup-forms/popup
/dyTracker.js?bust=release
/dynamic-yield/report/pageview
/egmont-ads
/egmont-continuous-scroll/continuous-scroll-analytics.js
/egmont-streamlined-ads
/elasticsuite/tracker
/emediate-responsive-wp-plugin
/empty.html$subdocument,domain=hotellorestaurang.se|byggfakta.today|omtanke.today|citymark.today
/enklare-banners/enklare-torgetgruppen
/entag.$script,domain=leta.se
/entryclick;_
/ess.eurovator.se/*
/eu_cookie_compliance$script,domain=industrinyheter.se|dagensnaringsliv.se|infrastrukturnyheter.se|sportochfritidsnyheter.se|inredningsnyheter.se|byggnyheter.se|dagensfastigheter.se|stockholmsbyggnyheter.se|energinyheter.se|vindkraftsnyheter.se|solenerginyheter.se|jarnvagsnyheter.se|transportochlogistik.se|metallerochgruvor.se|papperochmassa.se|miningmetalnews.com|visitskane.com|ergo.nu|ki.se|sxk.se
/evidon*.js$domain=morningstar.se
/exposure$xmlhttprequest,domain=lokalguiden.se
/expressen/crypt/?lpkey$all
/ext/phpbb/ads/*
/ezoic$domain=temadagar.se
/facebook_tracking_pixel$script
/fb_pixel.js
/featured/promotion$domain=borskollen.se
/filarkiv/bilderbanner/*
/firebase-analytics.js$domain=stoppapressarna.se
/flex-mag/js/dfp.js
/footer/ad|
/foretagarna.usercentrics.js$domain=foretagarna.se
/forumannons.$subdocument,image,script
/forum/assets/google-tag-manager
/forum/images/_banners
/forum/img/banners
/fptools.js$domain=allas.se|elle.se|femina.se|hant.se|mabra.com|residencemagazine.se|svenskdam.se|motherhood.se
/frontendLogger$domain=flashscore.se
/fullpageAd.js
/fullpage$script,domain=poddtoppen.se
/fullpage-ad.js
/fusionadloader.$script
/ga.js$domain=helgon.se
/ga_cookie_track.js
/gdprlock$third-party
/gdpr/*$domain=visitlulea.se|husbilskompisar.se|rotter.se|luleabusinessregion.se
/getAdById.php?
/getadd$domain=bovision.se
/get.aspx?AdSlotID$script
/glimr$script,domain=aftonbladet.se|blocket.se|livsstil.se|godare.se
/glimr-static$domain=~klart.se
/googleanalytics.js$domain=fria.nu|stockholmsfria.se
/google-analytics$domain=teknikveckan.se
/google-analytics-for-wordpress$important,script,xmlhttprequest
/google-analytics-premium$important,script
/google-gpt.js$domain=alekuriren.se
/google-tag-manager$domain=hemnet.se
/google-universal-analytics$script
/gpAnalytics$script
/gplus.php$script,domain=fria.nu|stockholmsfria.se
/gtagEventTracker.js
/gtm-sokande.js$domain=antagning.se|universityadmissions.se
/gtm-*.appspot.com
/headerbidding.js
/healthcare-puffar$domain=dh.se
/helios/multiad_jquery
/hemmafixbloggen/includes/events-tracker
/home/ads$domain=allastudier.se
/hotjar/hotjar.script.js
/hrnytt/banner$domain=hrnytt.se
/html5videovastplugin.js$domain=skidspar.se
/iab/iab.js
/idle.min.js$domain=180.se
/iframeadvloader.$script
/illustrationer/annons_
/images/site/annonser
/images/*casino$domain=festivalinfo.se
/img/allalanse$image,domain=ekonominyheter.se
/img/banklan/*$image,domain=ekonominyheter.se
/img/bettingstugan.$image
/img/compricer$image,domain=ekonominyheter.se
/impression$script,domain=affarsvarlden.se
/integrations/adwords$important,domain=dagen.se
/integrations/facebook-pixel$important,domain=dagen.se
/integrations/google-$important,domain=dagen.se
/isbanner/ib.js
/javascript_nbenhadverts/*
/jquery.smartbanner.js$domain=kristendate.se
/js/OneSignal.js
/js/PerimeterX$domain=skyscanner.se
/js/adLocker.
/js/annons.js
/js/byside_webcare
/js/external.php$domain=hockeysnack.com
/js/fullpageads.js
/js/iepngfix_tilebg
/js/improve_digital_ads
/js/infinite-ads
/js/intelecom.tracker
/js/sifo.js
/js/sticky-mobile-ad
/js/userneeds.
/jwpsrv.js$domain=aftonbladet.se|svd.se|tv.nu|axess.se|freeride.se|happyride.se|embed.futuresportsmedia.com|streamio.com|laget.se|moviezine.se|fasttrack.webstream.dk|cdn.jwplayer.com|livsstil.se|allas.se|elle.se|femina.se|hant.se|mabra.com|residencemagazine.se|svenskdam.se|motherhood.se|godare.se|recept.se|hastnet.se|skippo.se
/keremiya1/js/addtoany.js$script,important
/lasso-performance
/lazyad-loader.$script
/lazyload-ad.$script
/leeads-fullpage.js
/leeads_takeover$script
/linguee/statistics
/linkpulse/*$script
/links/*casino*.$domain=emocore.se
/live/radarmagazine.se.js
/loada.forum.$script
/load_ads.js$domain=koket.se
/logger/logger?
/logotyper/sponsorer-partners
/logs/client$domain=swebbtv.se
/log/hublytics
/log|$domain=booli.se
/log|$domain=vk.se|folkbladet.nu|nordsverige.se|mellanbygden.nu|vasterbottningen.se|lokaltidningen.nu
/losad/loada.$script
/maps.sponsored-pill.$script,domain=tripadvisor.se
/marbles/marbles.js
/marknadsguiden.$frame,domain=barometern.se|blt.se|bt.se|kristianstadsbladet.se|olandsbladet.se|smp.se|sydostran.se|trelleborgsallehanda.se|ut.se|ystadsallehanda.se|vxonews.se|vaxjobladet.se|nsk.se|klt.nu
/maxetise$domain=teknikveckan.se
/mb-admanager.js?
/media/eventad/*
/media/partners$domain=hockeynews.se|tvmatchen.nu
/mediehuset-gront/img/*annons
/mediehuset-gront/img/*banner
/meetrics-tracker
/mega.$domain=vk.se|folkbladet.nu|nordsverige.se|mellanbygden.nu|vasterbottningen.se|lokaltidningen.nu
/metrics$domain=swebbtv.se
/metrics/bambuser
/minbostadstatic/js/partner/*
/modal.js$script,domain=alltforforaldrar.se
/mod_carousel_banner$domain=bjuvsweek.se
/monetization/ads-module/*
/monetization/pixel-sdk/*
/mp_emediate/inc/annons.html
/mrbet_banner
/native$domain=sydnarkenytt.se
/native-ads$domain=atl.nu|landlantbruk.se|land.se
/native-article-campaigns$domain=allas.se|elle.se|femina.se|hant.se|mabra.com|residencemagazine.se|svenskdam.se|motherhood.se
/native.html$domain=allas.se|elle.se|femina.se|hant.se|mabra.com|residencemagazine.se|svenskdam.se|motherhood.se
/newsner-ad$domain=newsner.com|humorbibeln.se|sportbibeln.se|ettgottskratt.se|djurbibeln.se
/newsner-stats$domain=newsner.com|humorbibeln.se|sportbibeln.se|ettgottskratt.se|djurbibeln.se
/noview.$script,domain=trafikradion.com|gofm.se|trafik24.se
/nyhetsspalt_banner_js
/omniture/s_code.js
/one-signal$domain=swebbtv.se
/opus-analytics
/ordmedzcxy_files/ads$domain=ordmedzcxy.se
/pageView$xhr,domain=altinget.se
/pagead$domain=vilaser.se|horoskoptid.se|eniro.se
/pages/native$domain=aktuellhallbarhet.se|byggindustrin.se|dagensmedia.se|dagensmedicin.se|fastighetsnytt.se|resume.se|dagenssamhalle.se|market.se|dagligvarunytt.se|privataaffarer.se
/pages/tag$domain=aktuellhallbarhet.se|byggindustrin.se|dagensmedia.se|dagensmedicin.se|fastighetsnytt.se|resume.se|dagenssamhalle.se|market.se|dagligvarunytt.se|privataaffarer.se
/peertube-plugin-google-analytics
/permutive-async.js
/pfizer_analytics
/phaser-ads.min.js$script
/pixel/impression$domain=skyscanner.se
/playbuzz-ads-core
/player-plugin-ad$domain=tv.aftonbladet.se
/player-plugin-sponsor$domain=tv.aftonbladet.se
/player-plugin-tracking$domain=tv.aftonbladet.se
/plugins-mu/analytics
/plugins/add-to-any$script
/plugins/adlounge
/plugins/adsanity
/plugins/adsense%20click%20proctect
/plugins/ad-ace
/plugins/ad-blocking-advisor
/plugins/affiliate$script,domain=56kilo.se
/plugins/afp-default-pricetable/js/ga-tracking
/plugins/all-in-one-seo-pack$script
/plugins/analytics-insights
/plugins/angwp
/plugins/annonstorget$script
/plugins/appbanners/*
/plugins/ap-plugin-scripteo
/plugins/arscode-social-slider
/plugins/beautiful-and-responsive-cookie-consent$script,domain=melodifestivalklubben.se
/plugins/better-adsmanager/*$~stylesheet
/plugins/bfp-popup$script,domain=omtanke.today
/plugins/blog-analytics
/plugins/bmb-dfp-plugin
/plugins/borlabs-cookie$script,domain=alltombrollop.com
/plugins/boxzilla$script,domain=dialasen.com|arbetaren.se
/plugins/bravepopup$script,domain=matkasse.se|tidningenglobal.se|fempers.se
/plugins/bsa-plugin-pro-scripteo
/plugins/cardoza-facebook-like-box
/plugins/chimpy/*
/plugins/christmas-panda
/plugins/cm-pop-up-banners
/plugins/cm-takeover-ad
/plugins/complianz-gdpr$domain=iconmagazine.se|signprint.se|vilaser.se|arjeplognytt.se|aftonkuriren.se|tidningenglobal.se|tidningensyre.se|landetsfria.nu|fempers.se|macken.xyz|webb-tv.nu|kalmar.nu|brollopsmagasinet.se|megafonen.se|radiotreby.se|revisionsvarlden.se|kyrka.se|nuiroslagen.se|tlnt.se|sjofartstidningen.se|pensionarsliv.se
/plugins/consent-magic-pro$script,domain=namnmarkning.se|bluum.se|gobokhandeln.se
/plugins/content-hub-wp-plugin/assets/js/hub-time-spent
/plugins/convertplug
/plugins/convertpro
/plugins/cookie-law-info$script,domain=gilla.se|startaochdriva.se|sverige.nu|conpot.se|firstclassmagazine.se|magasinetkonkret.se|kvalitetsmagasinet.se|miljo-utveckling.se|telekomidag.se|vdtidningen.se|gullislastips.se|nyfiknainvesterare.se|discoveringtheplanet.com|bussmagasinet.se|torbjornstips.se|affarsstaden.se|marknadschefer.se|automation.se|dinbyggare.se|aktieskolan.se|insikt24.se|skogen.se
/plugins/cookie-notice$script,domain=bildobubbla.se|zeromagazine.nu|sverigespringer.se|gasetten.se|sillyseason.se|gentlemannaguiden.com|matmalin.se|svensktidskrift.se|schack.se|densistavilan.se|horisontmagasin.se|kobe.se|tidningenproffs.se|jaktojagare.se|tobaksfakta.se|bebisvarlden.se|underbaraclaras.se|cykelframjandet.se|dalabygden.se|lansposten.se|sormlandsbygden.se|vaguiden.se|grandtech.se
/plugins/cookie-popup$script,domain=skillingaryd.nu|xn--vrnamo-bua.nu
/plugins/cresta-social-share-counter
/plugins/custom-banners$domain=skolfamiljen.se
/plugins/daftplug-instantify$domain=se.moyens.net
/plugins/deblocker/js/deblocker$script,domain=~filecr.com
/plugins/dohi-sellbranch/js/popup$script
/plugins/doubleclick-wp
/plugins/dsgvo-tools-cookie$script,domain=motorsport4sale.com
/plugins/duracelltomi-google-tag-manager
/plugins/easy-adsense
/plugins/easy-affiliate-links
/plugins/easy-facebook-likebox$script
/plugins/easy-social-sharing$script
/plugins/elfsight-social-share-buttons
/plugins/embedpress/assets/js/ads.js
/plugins/exit-popup/*$script
/plugins/facebook-conversion-pixel
/plugins/facebook-ogg-meta-tags
/plugins/facebook-pagelike-widget
/plugins/facebook-popout-likebox
/plugins/fisher/core/js/generated/analytics.js
/plugins/fisher/core/js/generated/fixed-panorama
/plugins/fisher/core/js/generated/infinite-ads
/plugins/ga-germanized/*
/plugins/ga-in/*
/plugins/gdpr-cookie-compliance$domain=goteborgsgolfaren.se|nyhetersto.se|modernalivet.se
/plugins/genesis-simple-share$script
/plugins/ginger/addon/analytics/*
/plugins/google-analytics
/plugins/google-analytics-dashboard$important,script
/plugins/hemmafix-facebooklike
/plugins/host-analyticsjs-local
/plugins/hustle/*$script
/plugins/icegram
/plugins/iis-mailchimp
/plugins/interscroller-ads
/plugins/interstitial-ads
/plugins/jet-popup$domain=javligtgott.se
/plugins/jnews-social-share/*$script
/plugins/koko-analytics
/plugins/lbg-audio8-html5-radio_ads
/plugins/leeads-
/plugins/likebtn-like-button/*
/plugins/madonltd-full-screen-ad
/plugins/mailpoet/*$script,domain=~sameforeningen-stockholm.se
/plugins/mashshare
/plugins/material-admin/visitor-stats$script
/plugins/mediaconnect$domain=fof.se|spraktidningen.se|elinstallatoren.se|modernpsykologi.se|vvsforum.se
/plugins/metro-affiliate
/plugins/mitti-adform
/plugins/ml-adverts
/plugins/monsterinsights$script
/plugins/newsletter$script,domain=56kilo.se
/plugins/newsletter-leads/libs/simplemodal$script
/plugins/newsner-lead-tracking
/plugins/notificationx$script
/plugins/no-right-click-images-plugin$script
/plugins/ns-facebook-pixel
/plugins/official-facebook-pixel
/plugins/onesignal-free-web-push-notifications
/plugins/optin-cat-elite-wp$script
/plugins/page-views-count
/plugins/pc-google-analytics
/plugins/pixelyoursite
/plugins/pixel-caffeine
/plugins/pixel-cat
/plugins/popups/*$script,domain=svenskhistoria.se|bugburger.se
/plugins/popup$domain=ordfrontmagasin.se|snowmobile.se|forvaltarforum.se|it-finans.se|it-halsa.se|it-kanalen.se|it-pedagogen.se|it-retail.se|jobsinsweden.se
/plugins/pum-$script,domain=snowmobile.se|it-finans.se|it-halsa.se|it-kanalen.se|it-pedagogen.se|it-retail.se
/plugins/quantcast-choice$script,domain=handbollskanalen.se|javligtgott.se|dh.se
/plugins/quick-adsense
/plugins/r9-analytics
/plugins/random-banner
/plugins/sandviks-weblog$script,domain=bebisvarlden.se
/plugins/sassy-social-share/*$script,domain=~nova.rs
/plugins/sea-short-stats
/plugins/seo-automated-link-building
/plugins/se-wordpress-affiliatehelper
/plugins/share-and-follow/*
/plugins/simple-banner
/plugins/simple-social-buttons$script
/plugins/skydda-advisor
/plugins/socialsnap$script
/plugins/social-pug
/plugins/social-warfare$script,domain=varvat.se
/plugins/srs-simple-hits-counter
/plugins/statebuilt-facebook-page-like-popup
/plugins/sticky-facebook-banner$script
/plugins/super-socializer$script,domain=sportbilen.se
/plugins/svenskaspel-$script
/plugins/sw-ad-inserter
/plugins/sw_ad_inserter
/plugins/the-moneytizer/*$script
/plugins/thrive-leads
/plugins/trackable-social-share-icons
/plugins/triggerbee/*
/plugins/uk-cookie-consent$script,domain=cykla.se
/plugins/ultimate-social-deux$script,domain=totallyorebro.se|totallystockholm.se
/plugins/ultimate-social-media-$image,script
/plugins/ungrabber
/plugins/vizzit-analytics
/plugins/wccp-pro$domain=dinbyggare.se
/plugins/webtoffee-gdpr-cookie-consent$domain=forskning.se|hejaolika.se|kvartal.se|karriarlakare.se|svenskfilmdatabas.se|bredband.se
/plugins/wf-cookie-consent$script,domain=spelochfilm.se
/plugins/woocommerce-google-adwords
/plugins/wordpress-stats-manager-pro
/plugins/wplinktrade
/plugins/wpx-bannerize$script
/plugins/wp-adsense
/plugins/wp-analytify
/plugins/wp-auto-affiliate
/plugins/wp-banner-manager
/plugins/wp-click-info
/plugins/wp-content-copy-protection
/plugins/wp-copy-protect
/plugins/wp-evolve-gpt
/plugins/wp-facebook-pixel
/plugins/wp-gdpr-compliance$script,domain=pussad.se
/plugins/wp-lrf-paywall
/plugins/wp-popups-lite$domain=grillbaronen.se|spelochfilm.se|sameforeningen-stockholm.se|norrkopingshistoria.se
/plugins/wp-power-stats
/plugins/wp-snow-effect
/plugins/wp-statistics
/plugins/wp-stats-manager
/plugins/wysija-newsletters
/plugins/yeloni-free-exit-popup
/plugins/yuzo/public/assets/js/pixel-geo
/pogoadkit.js$domain=nordic.ign.com
/popup-subscribe.js$domain=borsvarlden.com
/popup/follow-us-fb
/prebid_rtb_call
/prisjakt$xmlhttprequest,domain=fz.se
/private-browsing.js$domain=thelocal.se
/prod/adform
/profile$ping,domain=feber.se|skippo.se|tasteline.com|tjock.se|veckorevyn.com|marcusoscarsson.se|handbollskanalen.se|surfa.se|nordichardware.se|hockeynews.se|tv4.se|fotbollskanalen.se|koket.se|teknikveckan.se|56kilo.se
/promoted_ads$domain=bostadsportal.se
/ps-partner$xmlhttprequest,domain=dagensps.se
/publicPartners$domain=familjehemsbanken.se|familjehemmet.se
/public/log$domain=kalender.se
/pulsetracking$script
/pum/*$domain=flm.nu|dagenslogistik.se|battrestadsdel.se|skaneplus.se
/qc_cmp$domain=reseguiden.se
/questback.popup$script
/rantekartan$subdocument,domain=expressen.se
/raven$script,domain=mitti.se|travnet.se|nyheter24.se|tyda.se
/recommendations$xmlhttprequest,domain=expressen.se
/registerhit?$image
/renderBanner.do?zoneId=
/resource.ifragasatt.se/sd-ads
/retargeting-pixels
/revive.js$domain=skidspar.se
/revive/revivejs.php$script
/revive/www/images$image
/rubiconproject_prebid
/scripts/js3caf.js
/scripts/leeads-
/scripts/opt/view.analytics.js
/script.js$3p,domain=spelkritik.se
/seenthis-hub$script
/se-ads-microservice
/se-calico/bundle.js
/se-ocelot/bundle.js
/se-recommendation-microservice$domain=allas.se|elle.se|femina.se|hant.se|mabra.com|residencemagazine.se|svenskdam.se|motherhood.se
/sg_reklam$domain=svampguiden.com
/sh404sefsocial$script
/sharedaddy/sharing.$script
/shared/crm-campaign-handler.js$script
/sharethis.js$domain=allsvenskan.se|superettan.se
/sidebar-ads
/siforesponsivemeasure
/sifo-tracking.js
/sifo_analytics
/sifo_msr
/site_media/annons
/skolvarlden_theme/js/s_code.js
/skrattnetdotse/js-ck.js
/skrattnetdotse/js-xdp.js
/smartBanner.js$domain=hant.se|svenskdam.se
/snowday262.js
/snowfall.jquery.min.js
/snowfall.min.jquery.js
/snowplow$script,domain=~rossmann.pl|~prolific.co|~nrk.no
/soledad/js/detector.js
/sounds/chimes.mp3$domain=skaneplus.se
/spec/adsm.macro.
/sponsoredLink.js$domain=fotbolltransfers.com
/sponsored_articles$domain=fastighetssverige.se
/sponsorloggor$domain=swehockey.se
/sponsors$domain=sdhl.se|storvretaibk.se|obosdamallsvenskan.se|elitettan.se
/spotlight-ad_$image
/ss_foundation/combined_li_tracking
/static.marklar.se/*-tracker
/static/js/loada.js
/static/media/*casino$domain=dagenstv.com|kolla.tv
/statistics/statistics.js
/statistics/statistics.php
/stats.wp.com$script
/stats/ewstats.
/stats/stats.asp?
/sticky-ads$script
/strossle-analytics.js
/strossle-start-page-ad$xmlhttprequest
/strossle-widget
/sunt/mainfeed
/sunt/sidefeed
/sveacasino_banner
/svenska-ridsportforbundet/*banners
/svff/bannerblock/*
/sv_se/metrics/*$script,xmlhttprequest
/swordfishinc.download.akamai.com/*$script
/synonymerse-adapter.js$domain=synonymer.se
/tabs_hits_counter.php$image
/takeover-ad.js$domain=ridsport.se
/takeover.js$domain=gekas.se
/tasteline/templates/popup
/tbilen/banner/*
/templates/ad_$domain=jaktojagare.se
/thumbnail_bettingstugan$image
/thumbs/webbannons$image
/tinypass-gtp.min.js
/toppbanner.js$domain=sydnarkenytt.se
/toppbanner_snippet_js
/torgen/banner.stat
/trace$xhr,domain=netflixguiden.se|radio.se
/trackers/SessionCam-tag
/tracker.php?do$image
/tracker/socket$domain=swebbtv.se
/tracking.php?aid=
/tracking/cts.js
/tracking/fpc.js
/track.js$domain=destination.se|sistaminuten.se
/track/view?webInteractiveId$image
/trafikfonden/*
/tvg-legacy-splash-redirector/public/t/*
/tvg-redirector/public/t/*
/tv/annons$domain=expressen.se
/tv/brand-studio$domain=expressen.se
/tv/sponsrat$domain=expressen.se
/twitter_count.php$domain=fria.nu|stockholmsfria.se
/ub-ads/*$script
/unica/html-banners
/uploads/annonser
/uploads/bilder/Banner/*
/uploads/bilder/Samarbetspartners
/upload/puff/*$domain=bergsmannen.se|tidningenbyggmaterial.se|tidningendacksnack.se
/usabilla$script
/users/2401/*$image,domain=ng.se
/user_behaviour_data$domain=skyscanner.se
/utag$script,domain=gaffa.se
/utag/aller-media
/vestigo$domain=momondo.se
/vgc/cdn/js/libs/ast/*$script,domain=aftonbladet.se
/videojs-preroll$domain=himlentv7.se
/videojs.ima.$domain=sportbladetplay.se|staylive.tv
/viewed$xmlhttprequest,domain=fotbolltransfers.com
/view_count/view.php
/view_count/view$domain=byggahus.se
/visit/v.js
/wdg/iab-active
/wds_nyhetsbrev_popup
/webbresurser/banner/*
/white_pixel.gif$domain=byggfakta.today
/wordads-classes/js/*
/workbox-offline-ga$domain=magasinetkonkret.se
/wpbm-banners/*$image
/wp-content/banners$image
/wp-content/plugins/addthis/*
/wp-content/plugins/easy-social-share-buttons$script
/wp-content/plugins/email-subscribe$script
/wp-content/plugins/top-10/*$script
/wp-content/static/unruly.js$script
/wp-content/themes/keremiya1/js/jopper.
/wp-content/themes/keremiya1/js/license.
/wp-content/themes/keremiya1/js/script.js
/wp-content/uploads/html5ads/*
/wp-content/uploads/*Casinodealen$image
/wp-content/uploads/*LeoVegas$image
/wp-content/uploads/*annons$image,domain=~datahjelperne.no|~dataliner.no|~annonsere.gulesider.no
/wp-content/uploads/*banner$image,domain=marsta.nu|alltomhif.se|branschkoll.se|brollopsmagasinet.se|bussmagasinet.se|danstidningen.se|guldkanalen.se|katerinamagasin.se|ljuskultur.se|sportpanelen.se|turismnytt.se|opulens.se|borattforum.se|dental24.se|tekniknytt.se|pakryss.se|investerarbrevet.se|svensktidskrift.se|electronic.se|restaurangvarlden.se|finanstid.se|naringslivetvgl.se|dalarnasaffarer.se|stockholmsaffarer.se|jamtlandsaffarer.se|hallandsnaringsliv.se|sjuharadsnaringsliv.se|battregolf.se|svenskhistoria.se|arjeplognytt.se|bioenergitidningen.se|fisheco.se|autonytt.se|zeromagazine.nu|improveme.se|dagensinfrastruktur.se|nordiskaprojekt.se|svenskbyggtidning.se|grontsamhallsbyggande.se|alekuriren.se|realtid.se|golfguidenonline.se
/wp-content/uploads/*betfair$image
/wp-content/uploads/*bethard$image
/wp-content/uploads/*bettingkollen$image
/wp-content/uploads/*bettingstugan$image
/wp-content/uploads/*betting$image,domain=nyadagbladet.se|kulturbloggen.com|hockeybladet.nu|newsvoice.se|spelochfilm.se|bandyfeber.com|battrestadsdel.se
/wp-content/uploads/*casinoutan$image
/wp-content/uploads/*casino$image,domain=nyadagbladet.se|kulturbloggen.com|newsvoice.se|svenskhistoria.se|battrestadsdel.se|zeromagazine.nu|totallyorebro.se|totallystockholm.se|djungeltrumman.se|vaken.se|tekniknytt.se|kingsizemag.se|spelochfilm.se|macken.xyz|improveme.se|bandyfeber.com|stoppapressarna.se|dagensinfrastruktur.se|nyaprojekt.se|nordiskaprojekt.se|svenskbyggtidning.se|grontsamhallsbyggande.se|sjostadsbladet.se|autonytt.se|hockeybladet.nu|tv-kanal.se
/wp-content/uploads/*kasino$image,domain=improveme.se|sjostadsbladet.se
/wp-content/uploads/*mrgreen$image
/wp-content/uploads/*ninjacasino$image
/wp-content/uploads/*noaccountbet$image
/wp-content/uploads/*oddsbonusar$image
/wp-content/uploads/*reklam$image,domain=hockeyettan.se
/wp-content/uploads/*svea-casino$image
/wp-content/uploads/*svenskacasinoonline$image
/wp-content/uploads/*unibet$image
/wp-content/uploads/*-sidebar$image,domain=dagensinfrastruktur.se|nyaprojekt.se|nordiskaprojekt.se|svenskbyggtidning.se|grontsamhallsbyggande.se
/wp-content/uploads/*/public/assets/js/advanced.js$script
/wp-content\/uploads\/[0-9]+/$script,domain=skanesport.se|dackavisen.se|automation.se|tidningenproffs.se|densistavilan.se|universitetslararen.se|alekuriren.se
/wp-json/wpstatistics
/wp-json/wp-statistics
/wp-native-ads.json
/ws-tracking$domain=voister.se
/ws-tracking.js$domain=tidningenbalans.se
/www.livsstil.se\/cnp-assets\/[0-9]+./$script,domain=livsstil.se
/www/images/*$domain=elektronikforumet.com
/xhr-ads.min.js
/xhr/b/s$domain=skyscanner.se
/zad.js$domain=nordic.ign.com
/zdadkit$domain=nordic.ign.com
/*banner-nyhetsbrev*.mp4
/?adsforwp_front_js
/?agg_url=/shopping$domain=nyheter24.se
/?agg_url=/sponsratinnehall$domain=nyheter24.se
/?client=ca-pub-$script
/?dtbnrspcid=$xmlhttprequest
/?file=lokus$subdocument
/?news=ajaxrequest&ArtSponsor
/?news=ajaxrequest&bannerlinks
/?news=ajaxrequest&bannerzone
/?news=ajaxrequest&blok=sliderBanner
/?template=prisjakt$domain=ljudochbild.se
/?trafikkalla$image,domain=bloggplatsen.se
/_adsmodern/*$image
/_api/*/visit$domain=placera.se
/_graphics/annons
/_papers_media/banners
/_sites_media/*/uploads/Banners
/_t/se.js$domain=hornbach.se
/_vercel/insights/*
://gtm.*.js?id=GTM
://gtm.*/g/collect?
://impression-tracker-service
://sifomedia.
?action=advanced-ads-tracking-track
?action=get_banners$domain=djungeltrumman.se
?autoPlay$frame,removeparam=autoPlay,domain=expressen.se
?autoplay=true$frame,removeparam=autoplay,domain=expressen.se
?url=*impse.tradedoubler.com$image
@@/adserver.$script,~third-party,domain=fotosidan.se|utsidan.se
@@/advert.js$1p,domain=aktuellhallbarhet.se|byggindustrin.se|dagensmedia.se|dagensmedicin.se|fastighetsnytt.se|resume.se|dagenssamhalle.se|market.se|dagligvarunytt.se|privataaffarer.se
@@/adx.js$~third-party,domain=atl.nu|landlantbruk.se|land.se
@@/ad-block-detection-script$domain=blocket.se
@@/aff/images/*$image,domain=alltforforaldrar.se
@@/appbanner.jpg$image,domain=guldkanalen.se
@@/assets/ads-dm.js$~third-party,domain=corren.se|folkbladet.se|mvt.se|nt.se|vt.se|vimmerbytidning.se|kuriren.nu|nsd.se|norran.se|pt.se|ekuriren.se|strengnastidning.se|kkuriren.se|sn.se|eposten.se|unt.se|helagotland.se|kindaposten.se|gotlandjustnu.se
@@/freemium/di/analytics$script,domain=di.se
@@/lazy_load.js?gcb$domain=hemmanytt.se
@@/plugins/ad-ace/*/adblock-detector
@@/plugins/convertplug/modules/modal/*/cross.png$image,~third-party
@@/scripts/advert_$~third-party,domain=di.se
@@_advert.$domain=e-pages.dk
@@||cargodisplayads.com/gota/api/v1/adImage$image,domain=barometern.se|blt.se|bt.se|kristianstadsbladet.se|olandsbladet.se|smp.se|sydostran.se|trelleborgsallehanda.se|ut.se|ystadsallehanda.se|vxonews.se|vaxjobladet.se|nsk.se|klt.nu
@@||cargodisplayads.com/till_minne/
@@||cdn.play.showheroes.com/part/partimage$image
@@||cdn.play.showheroes.com/part/rendered$media
@@||createsend1.com/css/
@@||feed.meltwater.com^$subdocument
@@||fwmrm.net/ad/g/$xhr,domain=tv4play.se|tv4.se|fotbollskanalen.se|koket.se
@@||fwmrm.net/crossdomain.xml$domain=embed.viaplay.com
@@||img.upsales.com^
@@||js.createsend1.com/js/jquery
@@||js.driftt.com^$domain=sanity.io
@@||klaviyo.com/media/js/public/klaviyo_subscribe.js$domain=solostove.com
@@||kritiker.se^$generichide
@@||marketo.com^*/form
@@||monetize-static.viralize.tv/viralize_player_content$script,xhr
@@||nuthymia-llc.ck.page/*/index.js$domain=nickwignall.com
@@||pages.upsales.com^
@@||www.googletagmanager.com/gtm.js$script,domain=elgiganten.se
||1terms.com^
||123on.com/images/pixel
||123on.com/logs
||123on.com/static/videojs.pulse
||172.104.145.13^
||ab.fastighetsvarlden.se^$script
||accesslnk.com^
||activate.social^$third-party
||activehosted.com^$third-party
||addrevenue.io^$third-party
||addsleeper.com^$third-party
||addtoany.com^$third-party
||adeprimo.se^$third-party
||adfenix.com^$third-party
||adhype-assets.com/images/*betting
||adhype-assets.com/images/*casino
||adhype.se/js/native
||adnordics.com^$third-party
||adonsales.com^$third-party
||adonstudio.com^$third-party
||adviral.s3.amazonaws.com/sponsored/
||advisa.se^$third-party
||advisible.com^$third-party
||ad.iplayer.org^$third-party
||affiliatable.io^$third-party
||affiliator.com^$third-party
||aff.bstatic.com^$third-party
||aftonbladet.se.*.$document
||agency360.io^$third-party
||ajs-assets.ftstatic.com/ftUtils.js
||akademiskahus.se/AddThis?$script
||alkemi.com.se^
||allaaktier.se/ads/
||allastudier.se/TrackingSearch
||allastudier.se/search-sponsor
||allsvenskan.se/allsvenskan-script-min.js
||alphalete.com.se^
||amazonaws.com/adn-tag
||amazonaws.com/adsfallback/
||amazonaws.com/metapic-cdn/*/metapic.
||amazonaws.com/pfe_im/js/prod/pcc/s_code.js
||analytics-smhise.smhi.se^
||analytics.barnebys.sh^$image
||analytics.gen.shield.monitoringservice.co^
||analytics.ozzi.io^$third-party
||analytics.teknikveckan.se^
||analytics.undeco.se^
||apis.google.com/js/plusone.js$third-party
||api-sa.rikatillsammans.se^
||api.hitta.se/creepy
||api.hitta.se/offer
||api.hitta.se/partnerintegration
||api.hitta.se/statistics
||api.mpzmail.com/tracker
||api.netb11.com/b/$image
||api.staylive.tv/videos/engagement
||applets.ebxcdn.com/ebx.js$domain=stoppapressarna.se
||applicationinsights.azure.com/*track
||app.termly.io^$domain=soderkopingsposten.se
||apsis.one^$third-party
||ascontentcloud.com^$third-party
||aservice.tools^
||assets.pinterest.com/js/pinit$third-party
||assets.tumblr.com/share-button.js$third-party
||assets.voyado.com/jsfiles/analytics
||assistanskoll.se/images/banner
||atl.nu/api/mnews
||atmtd.com^$third-party
||auction-release.mlpapi.com/site/LoadPluginSite
||aventyret.com^$third-party
||aweber.com^$third-party
||axess.se^*/track-views
||azurewebsites.net/partnerArticle
||bannerutbyte.se^$third-party
||barbours.com.se^
||barnebys.sh/js/btag
||bcm.interactives.dk/script/
||bellmetric.net^$third-party
||best-prizes-now.$all
||bettingstugan.se^$third-party
||biddercore.io^$third-party
||bilweb.se^$third-party
||biowebb-data.*.amazonaws$important,third-party
||bio.se/js/googleAnalytics.js
||bjuvsweek.se/images/*annons
||blocket.se^$third-party
||bloggportalen.se^*/blogstat.js
||blogg.se/plugin/ads.js
||blogg.se/public/js/metrics
||blogg.se/shared/js/bloggse.js
||bloglovin.com^$third-party
||bokmassan.se/wp-json/*/ad/
||boktugg.se/wp-content/cache/min/1/pa-
||bonniergaming.com^$third-party
||borsvarlden-banners.azurewebsites.net^
||borsvarlden.com/banners/
||borsvarlden.com/js/cookie-notice
||brandy.bonniernewslifestyle.se^
||breakit.se/js/ads/
||breakit.se/js/facebook
||breakit.se/js/google-analytics
||breakit.se/js/hotjar
||bstatic.com/static/affiliate$third-party,~stylesheet
||btcswe.com^$third-party
||buzzador.com^$third-party
||bwz.se^$third-party
||bytbil.com/bundles/js/tracking
||bytelab.dk^$third-party
||cargodisplayads.com^$third-party
||carneoam.com/advert/
||cartbooster.io^$third-party
||casinotoplists.com^$third-party
||casinoutankonto.net^$third-party
||casono.se^$third-party
||ccpa.sp-prod.net^$domain=m3.se|pcforalla.se|macworld.se|computersweden.se
||cdn-cookieyes.com^$domain=lokalti.se|jarnvagar.nu|senses.se|norrmejerier.se|temadagar.se|smartsenior.se|tekniknytt.se|nordigt.se|autonytt.se|vm-fotboll.se|kak.se|smhi.se|borattforum.se|mis.se|universitetslararen.se|em-fotboll.se|lakemedelsvarlden.se|samfalligheterna.se|husbilsplats.se|katerinamagasin.se|dagenslogistik.se|biostock.se|skellefteaworks.se|datormagazin.se|travnet.se|malarbok.nu|barn-filmer.se|matmenyer.se|sunnenytt.se
||cdn-sitegainer.com/sitegainer
||cdn.adt*/atag.js?$third-party
||cdn.adt*/jsTag?$third-party
||cdn.advisible.com/accl
||cdn.advisible.com/adk
||cdn.aller.se/cts/
||cdn.livechatinc.com/tracking$domain=~box.co.uk
||cdn.svenskalag.se/img/sponsors$image
||centotag.io^$third-party
||cervera.se/t/t?
||championsverige.com.se^
||cision.com^$badfilter
||cision.com^$third-party
||ck.page^$third-party
||cmp.radioplay.se^
||cmp.setupcmp.com^$domain=se.azrhymes.com
||cms.catena.media/js/cm-tracking
||cncptx.com^$third-party
||cncpt-central.com^$third-party
||cncpt.dk^$third-party
||collect.breakit.se^
||compado.com^$third-party
||compricer.se^$third-party
||connectio.s3.amazonaws.com/connect-retarget$script
||connect.facebook.net^$domain=friatider.se|fotosidan.se|ng.se|psykologiguiden.se|lektionsbanken.se|lajvo.se|kvinnatillkvinna.se|epochtimes.se|newsner.com|humorbibeln.se|sportbibeln.se|ettgottskratt.se|djurbibeln.se|sillyseason.se|loppi.se|kyrkanstidning.se|tn.se
||connect.nosto.com^*/behav-popup.$script
||consentframework.com^$domain=luleahockeyforum.com|se.moyens.net
||consentmanager.net^$domain=allastudier.se|gbgfotboll.se|stff.se|svenskfotboll.se|coop.se|dagens.se|mobil.se|kamerabild.se|prevent.se|utsidan.se|inpress.com|studentum.se|utbildning.se
||consent.podplay.com^
||converdiant.com^$third-party
||convertbox.com^$third-party
||convertful.com^$third-party
||convertkit.com^$third-party
||conviva.com^$third-party
||cookiebot.com^$domain=ng.se|swedroid.se|bax-shop.se|kurera.se|upplysning.se|mitti.se|circlek.se|findroommate.se|sakochliv.se|polistidningen.se|fokus.se|spraktidningen.se|varden.se|trafiken.nu|energi.se|sverigesnatur.org|kreditrapporten.se|sis.se|accentmagasin.se|allsvenskan.se|superettan.se|alltomarbetsmiljo.se|tco.se|totallyorebro.se|totallystockholm.se|enirobuddy.se|framtid.se|byggfaktadocu.se|husdjur.se|chalmers.se|elinstallatoren.se|ff.se|modernpsykologi.se|qx.se|vatternrundan.se|vvsforum.se|naturvetarna.se|skolporten.se|dust2.se|ehandel.se|byggvarlden.se|varldenidag.se|influens.se|omtanke.today|konsumentmagasinet.se|svenskelitfotboll.se|journalisten.se|fastighetsvarlden.se|jaktjournalen.se|friidrott.se|dagensps.se|vildmarken.se|kyrkanstidning.se|tmf.se|sokbat.se|bilkompaniet.se|driva-eget.se|hv.se|folkhalsomyndigheten.se|dinpsykiskahalsa.se|ekonomifakta.se|hyresbostader.se|rsyd.se|byggforetagen.se|vasterastidning.se|storyhouseegmont.se
||cookiehub.net^$domain=da.se
||cookieinformation.com^$domain=folkofolk.se|dental24.se|vinbanken.se|handelskammarenvarmland.se|enahabo.se|bostadsportal.se
||cookieinfoscript.com^$domain=webbkryss.nu
||cookielaw.org^$domain=cartoonnetwork.se|tv4.se|fotbollskanalen.se|koket.se|flashscore.se|ikea.com|recept.se|manpower.se|mtv.se|natgeotv.com|internetkunskap.se|internetstiftelsen.se|yelp.se|spisa.nu|viaplayradio.se|booli.se|svenskarnaochinternet.se|sv.bab.la|tripadvisor.se|sydkusten.es|livetochdiabetes.se|voister.se|nok.se|motesplatsen.se|thelocal.se|placera.se|infotorgjuridik.se|se.trustpilot.com|travronden.se|travrondenspel.se|hammarbyfotboll.se|pricerunner.se|billetto.se|lidl.se|pwc.se
||cookiepro.com^$domain=birthday.se|djurskyddet.se|havet.nu|svenskfast.se|fiskejournalen.se|upplysning.se
||cookietractor.com^$domain=innebandy.se|orientering.se|pluggakuten.se|munskankarna.se
||cookie-script.com/analytics
||cookie-script.com^$domain=axess.se|dagensjuridik.se|foodfolder.se|arkitektur.se|internetlankar.se|friluftsframjandet.se|lchfarkivet.se|bakasockerfritt.se|handelsradet.se|cirkulation.se
||covatic.io^$third-party
||createsend1.com^$third-party,~image
||createsend.com^$third-party
||curemedia.se^$third-party
||custosgroup.com^$third-party
||cxpublic.com^$third-party
||d1dy2xw1aqg7xq.cloudfront.net/seo_clickin_script
||d1ggib8p3xdn3u.cloudfront.net/script.js
||d1gwclp1pmzk26.cloudfront.net/agile/agile-cloud.js
||d2m8uxg4w7uelx.cloudfront.net/fpa.js
||d2m8uxg4w7uelx.cloudfront.net/fullpageads
||d2qrdklrsxowl2.cloudfront.net/js/hapyak.js
||d9v72urx9pbbc.cloudfront.net/LoadSlotLocator
||d9v72urx9pbbc.cloudfront.net/channel
||d10lumateci472.cloudfront.net/?amuld$script
||d11j2g8hmtmh4u.cloudfront.net/losad
||d11j2g8hmtmh4u.cloudfront.net/loswidget
||d11j2g8hmtmh4u.cloudfront.net/orion
||d11j2g8hmtmh4u.cloudfront.net/tags
||d16fx559zbp759.cloudfront.net/common
||d16fx559zbp759.cloudfront.net/sites
||d24rtvkqjwgutp.cloudfront.net/*yb.js
||d31djwpx7pcvsr.cloudfront.net/production/*/js/segment.js
||d2189b0dij3l7v.cloudfront.net/p/$domain=tv4play.se|tv4.se|fotbollskanalen.se|koket.se
||dackpartner-web.s3.amazonaws.com^$third-party
||deals.innocode.no^$third-party
||delivery.youplay.se/api/player_metrics?
||delivery.youplay.se/report?$image
||destination.se^$third-party
||didomi.nwtmedia.se^
||digitaliseringsinitiativet.se^
||digitaloceanspaces.com/ethical.min.js
||dinbilgaranti.se^
||distansarbete.com^
||diu127fbe6pn6.cloudfront.net^*/ga-universal.html
||doktor-se.onelink.me^$image
||driftt.com^$third-party
||drift.com^$third-party
||dsms0mj1bbhn4.cloudfront.net/assets/pub/shareaholic.$script
||dspk.kindredplc.com/renderImage.aspx$image
||eacdn.com/TrafficOpt/$script
||easyweb.se/stats/$image
||ebbot.eu/api/widget/analytics
||ecomm.events/i.js
||ekonomifakta.se/monitoring
||elfsight.com/events/views
||embed.lpcontent.net/leadboxes$script
||embed.viaplay.com/*autoplay=true$frame,removeparam=autoplay
||embi-media.com^$third-party
||emg-services.net/public/scripts/bundles/emg-desktop
||emg-services.net/public/scripts/bundles/emg-dfp
||emotorsport.se/ans/$image
||eniro.se/scoop.js
||entainpartners.com^$third-party
||episerver.net/*/epi-util/find.js
||es.loppi.se^
||etc.nu/ethical.min.js
||eugamblers.org^$third-party
||europe-west1-bonnier-big-data.cloudfunctions.net^$third-party
||eu-north-1.amazonaws.com/*images/*Banner
||events.forzasys.com/get.min.js
||evertiq.se/bimg/
||evidon.com^$third-party,domain=fasting.nu
||evt-api.ntm.eu/api/*/datacollector
||execute-api.eu-west-1.amazonaws.com/live/analytics
||existenz.se/img/o/
||exitintel.com^$third-party
||expekt.se^$third-party
||extellio.com^$third-party
||external.reseguiden.se/offer
||facebook.com/plugins/share_button$third-party
||facebook.com^*/plugins/like$third-party
||fakturino.se^$third-party
||familjehemsbanken.se/api/partners
||famobi.com/play/hit/
||fastout.com/analytics
||fasttrack.webstream.dk/statistik
||feedblitz.com^$third-party
||feeds.feedburner.com^$image
||feed.mikle.com^$third-party,domain=ekonominyheter.se
||filasverigese.com^
||fila.com.se^
||files.cdn.spilcloud.com/pb/$script
||filmtopp.se/upload/*/annons$image
||findit.fi/js/prebid
||flashback.org/rlog.php
||flirtmatch.se^
||fodertipset.se/cookie-info
||folkspel.se^$third-party
||footjoygolfskorrea.com.se^
||forms.hsforms.com^*/counters.$image
||forum.odla.nu/js/bonnier.js
||fotboll.com/*casino$image
||fraagesport.com^
||freewheel-mtgx-tv.akamaized.net^$media
||freyanews.com^*/tracker$script
||fritiden.se/js/cookiealert-standalone.js
||funnelytics.io^$third-party
||gamblersrules.com^$third-party
||gamblingsyndication.com^$third-party
||gamedistribution.com/libs/gd/analytics
||gamereactor.se/ads/
||gamereactor.se/exclusive.json
||gamesglue.com/js/gameanalytics/GameAnalytics
||gatekeeperconsent.com^$domain=hemmanytt.se|svenskaorduttryck.se|wernamaten.se|sanghafte.se
||getanewsletter.com/js-forms-assets/popups.js
||getlevelten.com^$third-party
||getsitecontrol.com^$third-party
||girohjalm.com.se^
||glitnoraffiliates.com^$third-party
||gnuheter.com/creeper/image
||googletagmanager.com^$important,domain=tradera.com|xxl.se|prisjakt.nu
||google-analytics.com^$important,domain=aftonbladet.se|tradera.com|xxl.se
||gopeach.se^$third-party
||gravito.net^$domain=hitta.se|gp.se|bohuslaningen.se|stromstadstidning.se|markposten.se|harrydaposten.se|partilletidning.se|sttidningen.se|molndalsposten.se|kungalvsposten.se|kungsbackaposten.se|alingsastidning.se|ttela.se|hallandsposten.se|hn.se|mellerudsnyheter.se
||grillbloggen.nu/media/com_rstbox/js/engagebox.js
||growthbook.io^$domain=allas.se|elle.se|femina.se|hant.se|mabra.com|residencemagazine.se|svenskdam.se|motherhood.se
||gstatic.com/partners/badge$subdocument
||gtm.ekonomifakta.se^
||gtm.findroommate.dk^
||guesssverige.com.se^
||gymshark-sweden.com.se^
||hajper.com^$third-party
||happygreen.se^$third-party
||hapyak.com^$third-party
||harmonious-station-to-station.podplay.com/script.js
||hastnet.se/adtech
||hejauppsala.com/*banner$image
||helix.svt.se/events
||helloreco.com^$third-party
||heroaffiliates.com^$third-party
||herokuapp.com/visit?$image
||hittahem.se^$third-party
||hltv.org/js/ht.$domain=dust2.se
||hockeysnack.com/pagespeed_static/1.$image
||hoomemakleri.se^$third-party
||humorbrevet.se/externa_bilder
||iconosquare.com^$third-party
||ifragasatt.se/stats/
||images-ads.aland.com^
||images.woo.a2d.tv/creative_assets$image,domain=tv4play.se|tv4.se|fotbollskanalen.se|koket.se
||imasdk.googleapis.com/js/sdkloader/ima3.js$script,redirect=google-ima.js,important,domain=screen9.com|atl.nu
||imgix.net^*/analytics.$script
||imgsct.cookiebot.com/1.gif
||img.upsales.com/*/visit$script,important
||imp.laget.se^
||inboxads.com^$third-party
||inmobi.com^$domain=alltomelbil.se|rikatillsammans.se|egoinas.se|land.se|moviezine.se|travelnews.se|varldenshaftigaste.se|merinfo.se|foreca.se|matklubben.se|reseguiden.se|newsner.com|humorbibeln.se|sportbibeln.se|ettgottskratt.se|djurbibeln.se|laget.se|byrum.se|sportlovin.se|receptfavoriter.se|forni.se|kimura.se|cornucopia.se|norrahalland.se|elevspel.se|finanstid.se|tittapavideon.se|motormagasinet.se|food-supply.se|dagenshandel.se|plastnet.se|habit.se|woodnet.se|foodnet.se|transportnet.se|processnet.se|packnet.se|verkstaderna.se|medtechmagazine.se|recyclingnet.se|rt-forum.se|uochd.se|lifesciencesweden.se|fri-kopenskap.se|cleannet.se|metal-supply.se|framtidensbygg.se|entreprenad.com|mykitchenstories.se|cancelculture.se|mytaste.se|findit.se|lchfarkivet.se|brinkenbakar.se|foretagande.se|fotbolltransfers.com|affarsvarlden.se|villalivet.se|branschaktuellt.se|nordic.ign.com|fragbite.se|lindasbakskola.se|jennysmatblogg.nu|filippoon.se|lesscarbs.se|eniro.se|matspar.se|xnytt.se|alltomkungligt.se|swehockey.se|vackertvader.se|newly.se|nyheter2.se
||insertcoin.se^$third-party
||insplanet.com^$third-party
||instaforex.com^$third-party
||instiengage.com^$domain=stoppapressarna.se
||intagme.com^$third-party
||interactiveads.ai^$third-party
||internetmedicin.se/log.php
||investerarbrevet.se^$third-party
||iphonecasinon.com^$third-party
||isgprivacy.cbsi.com^$domain=nickelodeon.se
||jajja.com^$third-party
||jenkler.se^$domain=uex.se
||jitsu.com/p.js
||jobba-hemifran.com^
||jobb.blocket.se/blocket_puff.html
||jobb.blocket.se^*/tracker.js
||jobb.blocket.se^*/xtcore.min.js
||jobtip.se^$domain=shortcut.se
||jst.ai^$third-party
||js.adsaga.se^$third-party
||js.evtr.nordiskemedier.dk^
||js.hs-banner.com^
||js.rating-widget.com/external
||juicer.io/api/page_views
||jwpcdn.com/player/plugins/inference/
||jwpcdn.com/player/*/bidding.js$domain=allas.se|elle.se|femina.se|hant.se|mabra.com|residencemagazine.se|svenskdam.se|motherhood.se|recept.se
||jwplayer.com/*/advertising$domain=allas.se|elle.se|femina.se|hant.se|mabra.com|residencemagazine.se|svenskdam.se|motherhood.se
||k5a.io^$script,redirect=noop.js,domain=tv2.no
||kajabi-cdn.com^$domain=nillaskitchen.com
||kalender.se/analytics
||kamrat.com/js/cookiescript
||kayak.xno.se^$script
||keenstockholm.com.se^
||kingsizemag.se/content/
||kingsizemag.se/kingrev.php
||kingsumo.com^$third-party
||klaviyo.com^$third-party,domain=~kmail-lists.com|~myklpages.com
||kolozzeum.com/forum/kollos$script
||konzilo.com/mtc.js
||konzilo.net/mtc.js
||kortio.se^$third-party
||kritiker.se/js/gdpr.js
||kundvisaren.se^$third-party
||kyrkanstidning.se/firstvisit$xhr,empty
||laget.se^*/retarget.js
||lajvo.se/addImpression
||lanapengar.expressen.se^
||lantbruksnet.se/files/reklan/
||lantbruksnytt.se/includes/$subdocument
||laromedia.se/Annonssystem/
||lasso.link^$third-party
||leadconnect.ipmaxi.se^$third-party
||leadenhancer.com^$third-party
||leazard.io^$domain=varmepumpsforum.com
||libring.com^$third-party
||lib.atomik.vip/loader.min.js
||lifeofsvea.se/production/borka/
||lifeofsvea.se/production/losjs/
||lifestyle.expressen.se^$subdocument
||likebtn.com^$third-party
||liveagent.se/scripts/track
||live-tag.creatopy.net^$third-party
||ljudoljus.net/images/banner/
||logsnag.com^$third-party
||logs.sesamy.com/events
||lokalguiden.se/magasinet/banner
||lok.se/pic/sponsor/
||longchampstockholm.com.se^
||lookaside.fbsbx.com/lookaside/crawler/
||look.ufinkln.com^
||look.utndln.com^$all
||lwadm.com^$important,domain=sydostran.se
||lwcdn.com/vendor/ima.min.js$script
||lystra.se^$third-party
||m1.analytics.sitevision-cloud.se^
||mailchimp.com^*/popup$script
||mailerlite.com/*/universal/*popups.js
||mailerlite.com^$third-party,domain=vandringsguiden.se|flm.nu
||mailmunch.co^$third-party,domain=affarsstaden.se|enkelteknik.se
||mailmunch.co^*/scrollbox$script
||makeinfluence.com^$third-party
||manatee.dk^$third-party
||manatee.io^$third-party
||marfeelcache.com^$third-party
||marketo.com^$third-party
||masture.mobi^
||matchads.net^$third-party
||matchesfashion.com^*/ExternalBanners
||matorama.se^$csp=img-src 'self' *.wordpress.com *.wp.com *.gravatar.com
||maxetise.net^$script,redirect-rule=noop.js,domain=feber.se|tjock.se
||mcgtrack.herokuapp.com^$third-party
||mediacreeper.com/image$image,redirect=32x32.png
||mediacreeper.se/image$image,redirect=32x32.png
||mediakraft.se^$third-party
||mediaserver.gvcaffiliates.com.cdn.cloudflare.net^
||media.arto.se/*annons$image,domain=natursidan.se
||media.dagensps.se/*banner$image
||media.golfbladet.se/*banner
||media.jw-it.se/b/$image
||media.jw-it.se/getip.php
||mediekompaniet.com^$third-party
||meltwater.com^$third-party
||metalcentral.net/images/*banner
||metapic.se^$third-party
||metromode.se/widget/club/
||mikz.com^$third-party
||miljomat.se/annonser
||missaffiliate.com^$third-party
||misssite.com/*/published-site-analytics.js
||mis.se/count/
||mitti.se/agstatistics-
||mitti.se/click-
||mogenromantik.com^
||momondo.se/*gtm/
||mraffiliate.com^$third-party
||mtpc.se^$third-party
||mtst.io/js/mtst.js
||multibrandaffiliates.com^$third-party
||myadmessenger.com^$third-party
||mymediaindex.com^$third-party
||narkive.se/ajax/Telem
||network-n.com^$third-party
||newsharecounts.*.amazonaws.com/nsc.js
||newstag.com/t/e$xmlhttprequest
||newstats.blogg.se^
||ng.se/nodecounter/
||nichehuset.dk^$third-party
||nitroscripts.com^
||nitroz.se/banners.min.js
||nordiskemedier.dk/banner/
||nordiskemedier.dk/bnr/
||nordiskemedier.dk/remodal$script
||nordiskskog.se/dynamic/serve.php
||norstatsurveys.com^$third-party
||notedmedia.se/pixel/
||nouw-ms-blog.azurewebsites.net/api/blogstatistic
||nouw.com/api/campaignpost
||nouw.com/api/postimpression
||nouw.com/api/postview
||nouw.com/campaignpost/reg/
||nuance.com/tagserver/logging
||nucleusanalytics.io^$third-party
||nyheteridag.se/ads/
||nyhetersto.se/webpushr-sw
||oas.*.se/om/$script
||obj.fotosidan.se/obj/pa/$image
||offer-go.com^$third-party
||onesignal.com^$domain=samnytt.se|battrestadsdel.se|beernews.se|ungdomsfotboll.se|rabattsok.se|1x2.se|cannabis.se|dackavisen.se|driva-eget.se|skogsaktuellt.se|maskinbladet.se|entreprenadaktuellt.se|ja.se|newsner.com|humorbibeln.se|sportbibeln.se|ettgottskratt.se|djurbibeln.se|finanstid.se|fokus.se|gasetten.se|fotbollsthlm.se|macken.xyz|naringslivetvgl.se|dalarnasaffarer.se|stockholmsaffarer.se|jamtlandsaffarer.se|hallandsnaringsliv.se|sjuharadsnaringsliv.se|netflixguiden.se|nyadagbladet.se|oskarshamns-nytt.se|swebbtv.se|thepattayanews.se|vaken.se|aktieskolan.se|fastighetsvarlden.se|mcparken.se|gaffa.se|alltomnorrtalje.se|morotsliv.com|it-finans.se|it-halsa.se|it-kanalen.se|it-pedagogen.se|it-retail.se|skaneplus.se|mittforetag.com
||onetrust.com^$third-party,domain=lantmannen.se
||online.bookvisit.com^$third-party,domain=campingsverige.se
||online.swedbank.se.swedd.$document
||onrender.com/tracker.js
||open-analytics.se^$third-party
||opinionstage.com/assets/autoengage.$script
||optmn.cloud/hb/
||optnmnstr.com^$third-party
||opulens.se^$csp=worker-src 'none'
||organicfruitapps.com/analytics
||owa.agriprim.se^
||pafpartners.com^$third-party
||palmangelssverige.com.se^
||pcf.tdscd.com^
||peertube.se^$frame,redirect=click2load.html,domain=nordiskradio.se
||pensiono.se.$subdocument
||pensiono.se^$third-party
||petrk.com^$third-party
||pheegoab.click^
||piano.io^$domain=thelocal.se|illvet.se|iform.se|varldenshistoria.se|popularhistoria.se|dagen.se|gds.se|slakthistoria.se|digitalfotoforalla.se
||pingback.issuu.com/ping
||pipedrive.com^*/statistics/seen
||pixel.bet^$third-party
||pixel.playbuzz.com^
||pji.nu/libs/pjpixel
||pji.nu^$third-party,domain=minhembio.com|ljudochbild.se
||platform.linkedin.com^$third-party
||platform.tumblr.com/*/share.js$third-party
||platssajten.se^$third-party
||plausible.io^$script,redirect-rule=noop.js,domain=feber.se|tjock.se
||plausible.webfokus.no^$third-party
||player.vimeo.com^$frame,redirect=click2load.html,domain=breakit.se
||pliing.com^$third-party
||plowking.mecenat.com^
||pm.azerioncircle.com^
||podcasts.nu/adbg.svg
||poddtoppen.se/api/ad?
||pomu.se/api/ads.json
||pomu.se/games/visit/
||portalhc.com^$third-party
||pricerunner.com/publisher-widgets$third-party
||prisjakt-a.$third-party,domain=~prisjakt.nu|~prisjakt.no|~pricespy.co.uk|~ledenicheur.fr|~prisjagt.dk|~pricespy.co.nz|~hintaopas.fi
||prisjakt.nu^$third-party
||prismic.io/prismic-toolbar$domain=alltomarbetsmiljo.se
||privacypolicies.com^$domain=fl-net.se
||privacy-center.org^$domain=180.se|agriaffaires.se|truckscorner.se|machineryzone.se|stegforhalsa.se|netdoktor.se|netdoktorpro.se|news55.se|hastnet.se
||privacy-mgmt.com^$domain=radio.se|dagenstv.com|kolla.tv|computersweden.se|woxikon.se|kokaihop.se|dagen.se|filmtopp.se|upday.com|gaffa.se
||prod.uidapi.com^$domain=tittapavideon.se
||proff.se^$third-party
||proxyas.com^$third-party
||prvcy.vkmedia.se^
||prylguiden.expressen.se^
||ptm.flowplayer.com^*/display$xmlhttprequest
||ptm.flowplayer.com^*/ping$xmlhttprequest
||ptm.flowplayer.com^*/view$xmlhttprequest
||pt.dwcdn.net/*/datawrapper.gif
||pushcrew.com^$third-party
||pushnice.com^
||pushpushgo.com^$third-party
||pushwhy.com^
||pxl.host^$third-party
||qimtek.se^$third-party
||quantcast.com^$domain=flashback.org|babyhjalp.se|nyadagbladet.se|enkelteknik.se|travelgrip.se|samnytt.se|nyteknik.se|lag-avtal.se|arbetarskydd.se|leta.se|motivation.se|sporttv.nu|goforfit.se|expo.se|poddtoppen.se|langd.se|doon.se|garaget.org|nouw.com|listor.se
||qx.se/view.php$image
||rabble-res.cloudinary.com^$third-party
||radio.se/iomm
||ramses.nu^$third-party
||raygun.io^$domain=koket.se
||reaktion.se^$third-party
||recirculation.spot.im^$third-party
||reco.se/widget/analytics
||reddit.com/static/button$third-party
||redeal.se^$third-party
||referralhero.com^$third-party
||rejsa.nu/ann$image
||rekai.se^$third-party,domain=folkpool.se
||rektek.se/widget/extraexposurejobs$third-party
||rek.ai^$third-party,domain=ng.se
||researchonline.se^$third-party
||reseguiden.se^$third-party
||reseguiden.se^*/google-tag
||resources.blogblog.com^*/paging_dot.$image
||resultify.com^$third-party
||resultify.se^$third-party
||res.cloudinary.com/internetmedicin/image/*/friends/
||res.se/js/ad.js
||revrelations.com^$third-party
||richmediastudio.com^$third-party
||riedta.com^$third-party
||routy.app^$third-party
||royapp.com^$third-party
||rpofsweden.com^
||rpofsweden.se^
||runtnc.net^
||salesiq.zoho.com/widget$domain=seodesign.se
||salesmanago.pl/api/push/notification$domain=aikfotboll.se
||salesmanago.pl/*popup$domain=land.se
||sales.agriprim.com/Banners
||sannsyn.com^$third-party
||sa.svenskalag.se/*/__tm.gif
||scandicpartners.se^$third-party
||schibsted.com/pulse$domain=aftonbladet.se
||script.e-space.se^$third-party
||sdk.mrf.io/statics/marfeel-sdk
||sdk.pulse.schibsted.com^$script,domain=aftonbladet.se|omni.se|omniekonomi.se|svd.se|prisjakt.nu
||seenthis.se^$third-party
||selectofmychoices.com^
||sellingsimplified.net^$third-party
||seonify.com^$third-party
||servg1.net^$third-party
||service.force.com^$domain=allabolag.se
||se-affiliate-gallery.aws.aller.com^
||shareaholic.com^$third-party
||shareaholic.net^$third-party
||sharedcount.com^$third-party
||sharethis.com^$third-party
||sitegainer.com/jsinsert/*/sitegainer$third-party
||skk.se/TSPD/
||skogsforum.pro/analytics
||skogsforum.se/async
||skogsforum.se^$csp=worker-src 'none'
||sleeknote.com^$third-party
||smartstats.kla.tv^
||snapwidget.com/images/snapwidget_ad
||snt-matrix-app.herokuapp.com^*/user-tracking
||solidtango.com^*/player_statistics$image
||spania.no^$third-party
||spelguiden.samnytt.se^
||spelhubben.se/?_dnembed$script
||spel.expressen.se^
||sporttv.nu/images/BetLogos
||sporttv.nu/images/sponsor/
||sporttv.nu/js/partners
||sprida.se^$third-party
||sprinkletxt.com^$third-party
||sp.tinymce.com^$image
||srvrtools.com/r/p.html?$subdocument
||srvrtools.com/t.js?
||stackpathcdn.com^*/shrMain$script
||stadiumstage.com^$third-party
||stallet.se/scripts/bx-abd.js
||static.hupso.com/share/js/counters.js
||statisticplatform.com^$third-party
||stats2.ehandel.se^
||stats.blogg.se^$image
||stats.docu.info^
||stats.easyweb.se^$third-party
||stats.ehandel.se^
||stats.helsingborg.se^
||stats.jibber.social^
||stats.playoncenter.com^
||stats.poddtoppen.se^
||stats.proff.se^
||stats.tipser.com^$xmlhttprequest
||stat.modette.se^
||stayfriends.de/metatag
||step.dk^$third-party
||stm.eniro.se^
||stockholmtarot.se^$third-party
||storage.googleapis.com/didna$third-party
||storymedia.se^$third-party
||streamio.com/api/*/stats$xmlhttprequest
||studads.com^$third-party
||suntana.se^$third-party
||susnet.*/susnetstat.js$script
||svd.se/api/dr-edition-teasers
||svd.se/api/live-ads/
||svenskafans.com/menu-logo/bottom
||sv.picmix.com/sw.js
||sv.picmix.com^$csp=worker-src 'none'
||s.arclk.net/tr?$all
||tally.so^$domain=tranakampsport.se
||tc.hometogo.net^$image
||telemetry.bambuser.io^
||tibaco.net/scripts/tws.js
||toolcontentcloud.com/*/asjs$domain=bredband.se
||top100ruokablogit.com^$third-party
||topblogarea.se/tracker
||toppmarkensverige.com^
||tourn.co^$third-party
||tourn.se^$third-party
||tracking.bonnier.news^
||tracking.fasab6f.se^
||track.intersport.se^
||track.postkodlotteriet.se^
||track.yetric.app^
||tradehouse.media^$third-party
||travellink.se/marketing-channel
||travronden.se/monitoring
||travtjansten.se^$third-party
||trckr*.nordiskemedier.dk^
||tripadvisor.se/PVLog
||tripadvisor.se/data/*/rum
||tripadvisor.se^$csp=worker-src 'none'
||tr.apsisforms.com^$third-party
||turistmal.se/js/popup-controller.js
||tv4.video-tracking.a2d.tv/anonymous/event
||tvmatchen.nu/plugins/splash-redirector
||tvmatchen.nu^*/smartbanner
||tvm-tv4-freewheel.akamaized.net^
||twingly.com^$third-party
||twitcount.com^$third-party
||t.atmng.io^
||t.elasticsuite.io^$third-party
||t.fml.rip^$third-party
||t.raptorsmartadvisor.com^$image
||ubembed.com^$third-party
||ues.vk.se^*/events
||ufinkln.com/offer?prod$popup
||umami.nordiskehandel.cloud^
||upsales.com^$third-party
||usabil.nu/media/*/casino$image
||usefathom.com^$domain=fz.se|sweclockers.com
||usercentrics.eu/1.gif
||usercentrics.eu/uct?$image
||usercentrics.eu^$domain=hemnet.se|kantarsifo.se|foretagarna.se
||userneeds.com^$third-party
||valentinosverige.com^
||vejaskor.com.se^
||vejasskor.com^
||viadata.store^$third-party
||viagogo.se^
||viforetag.se^$third-party
||vinguiden.com^$third-party
||viralize.tv/t-bid
||viralize.tv^$domain=tyda.se
||vovve.net/i/sponsorer
||voyager-widgets.aftonbladet.se/widgets/sports
||walls.io^$domain=svensktgolfforum.se
||wayke.se^$third-party,domain=siljannews.se
||wct-1.com^$third-party
||wct-2.com^$third-party
||webbannons.ntm.eu^$subdocument
||webbjobb.io^*/abb-$script
||webformscr.com/apps/fc3/build/default-handler.js
||webpower.eu^$third-party
||webpushs.com^$third-party
||websta.me^$third-party
||widgets.bonniernewslifestyle.se^$subdocument
||widgets.getpocket.com^$third-party
||widgets.jobtechdev.se^$third-party
||widget.getyourguide.com^$third-party
||widget.matklubben.*/tracker
||widget.mytaste.*/blogcounter
||widget.playoncenter.com/newplayer/js/pb_$script,redirect=noop.js
||wisepops.com^$third-party
||wishpond.net^$third-party
||woomio.com/assets/js/analytics
||workhaus.se^$third-party
||yelp.se/sit_rep
||yieldwrapper.com^$third-party
||youbora.com^*/sp.min.js$important,domain=aftonbladet.se|svd.se|livsstil.se|godare.se|tv.nu
||youtube.com/embed$frame,redirect=click2load.html,domain=ordfrontmagasin.se
||youtube.com/embed/*autoplay$subdocument,removeparam=autoplay,domain=kritiker.se
||ysektionen.se/media/uploads/*banner$image
||znaptag-tags-se.s3.amazonaws.com^$script
||zoho.com/hub/js/WebsiteAutomation.js$third-party
||zummycloud.com^$third-party
||zummy.io^$third-party
!#if env_chromium
||fast.fonts.com/t/1.css
||fast.fonts.net/t/1.css
||fast.fonts.net/lt/1.css
!#endif
!#if env_mobile
##.banner--mobiletoppanorama
##.mobile-homepage-ad
##.mobile-main-ad
##.mobil-annons
###mobile-banner-top
###mobile-banner-after-content
###mobile-banner-bottom
##div.mobile-ads-wrapper
##div.top-mobile-ad
##div.mobileads
##div.big-mobile-ads
##div#topBannerMobile
!#endif
!#if !env_chromium
||fast.fonts.net/*/1.css$domain=arkitekt.se|axess.se|diabetes.se|sverigeslarare.se|ljuskultur.se|electronic.se
branschkoll.se,rocknytt.net,upphandling24.se,kimura.se,datormagazin.se,villalivet.se,classicmotor.se,tidningenhalsa.se,husohem.se,guiden.se,nyadagbladet.se,enkelteknik.se,stoppapressarna.se##^script[id^="advanced-ads"]
branschkoll.se,rocknytt.net,upphandling24.se,kimura.se,datormagazin.se,villalivet.se,classicmotor.se,tidningenhalsa.se,husohem.se,guiden.se,nyadagbladet.se,enkelteknik.se##^script[id^="advanced_ads"]
branschkoll.se,rocknytt.net,upphandling24.se,kimura.se,datormagazin.se,villalivet.se,classicmotor.se,tidningenhalsa.se,husohem.se,guiden.se,nyadagbladet.se,enkelteknik.se##^script[id^="advads"]
branschkoll.se,rocknytt.net,upphandling24.se,kimura.se,datormagazin.se,villalivet.se,polistidningen.se,densistavilan.se,classicmotor.se,tidningenhalsa.se,husohem.se,guiden.se,nyadagbladet.se,enkelteknik.se##^script:has-text(advanced_ads)
branschkoll.se,rocknytt.net,upphandling24.se,kimura.se,datormagazin.se,villalivet.se,polistidningen.se,densistavilan.se,classicmotor.se,tidningenhalsa.se,husohem.se,guiden.se,nyadagbladet.se,enkelteknik.se##^script:has-text(advads)
stoppapressarna.se##^script[data-src*="advads"]
temadagar.se,lchfarkivet.se,wernamaten.se,sanghafte.se##^script:has-text(__ez)
svt.se###nyh_a11y-primary-navigation-list:style(float:unset!important;)
!#endif
!#if !env_mobile
/assets/js/modules/plugins/smoothPageScroll
/rokophoto-lite/js/SmoothScroll
/wp-enqueue/*smoothscroll
/themes/*/js/smoothscroll
/jquery.smoothwheel/*
/tapatalkdetect$script,1p
/themes/Jaz/inc/js/*nicescroll
/smart-app-banner*/banner.js
lundagard.se,boktugg.se,morotsliv.com,affarsstaden.se,kurera.se,nyfiknainvesterare.se##+js(aeld, wheel)
home2tiny.se##+js(aeld, /mousewheel|DOMMouseScroll/, smoothScrollEvent)
!#endif

```

### YouTube shorts

```
! Title: Hide YouTube Shorts
! Description: Hide all traces of YouTube shorts videos on YouTube
! Version: 1.9.0
! Last modified: 2024-02-17 11:55
! Expires: 2 weeks (update frequency)
! Homepage: https://github.com/gijsdev/ublock-hide-yt-shorts
! License: https://github.com/gijsdev/ublock-hide-yt-shorts/blob/master/LICENSE.md

! Remove empty spaces in grid
www.youtube.com##ytd-rich-grid-row,#contents.ytd-rich-grid-row:style(display: contents !important)

! Hide all videos containing the phrase "#shorts"
www.youtube.com##ytd-grid-video-renderer:has(#video-title:has-text(/(^| )#Shorts?( |$)/i))
www.youtube.com##ytd-rich-item-renderer:has(#video-title:has-text(/(^| )#Shorts?( |$)/i))

! Hide all videos with the shorts indicator on the thumbnail
www.youtube.com##ytd-grid-video-renderer:has([overlay-style="SHORTS"])
www.youtube.com##ytd-rich-item-renderer:has([overlay-style="SHORTS"])
www.youtube.com##ytd-video-renderer:has([overlay-style="SHORTS"])
www.youtube.com##ytd-item-section-renderer.ytd-section-list-renderer[page-subtype="subscriptions"]:has(ytd-video-renderer:has([overlay-style="SHORTS"]))

! Hide shorts button in sidebar
www.youtube.com##ytd-guide-entry-renderer:has(yt-formatted-string:has-text(/^Shorts$/i))
! Tablet resolution
www.youtube.com##ytd-mini-guide-entry-renderer:has(.title:has-text(/^Shorts$/i))

! Hide shorts section on homepage
www.youtube.com##ytd-rich-section-renderer:has(#title:has-text(/(^| )Shorts( |$)/i))
www.youtube.com##ytd-reel-shelf-renderer:has(.ytd-reel-shelf-renderer:has-text(/(^| )Shorts( |$)/i))

! Hide shorts tab on channel pages`
! Old style
www.youtube.com##tp-yt-paper-tab:has(.tp-yt-paper-tab:has-text(Shorts))
! New style (2023-10)
www.youtube.com##yt-tab-shape:has-text(/^Shorts$/)

! Hide short remixes in video descriptions
www.youtube.com##ytd-reel-shelf-renderer.ytd-structured-description-content-renderer:has-text(/^Shorts remixing this video$/i)

! Hide shorts category on homepage and search pages
www.youtube.com##yt-chip-cloud-chip-renderer:has(yt-formatted-string:has-text(/^Shorts$/i))

!!! MOBILE !!!

! Hide all videos in home feed containing the phrase "#shorts"
www.youtube.com##ytm-rich-item-renderer:has(#video-title:has-text(/(^| )#Shorts?( |$)/i))

! Hide all videos in subscription feed containing the phrase "#shorts"
m.youtube.com##ytm-item-section-renderer:has(#video-title:has-text(/(^| )#Shorts?( |$)/i))

! Hide shorts button in the bottom navigation bar
m.youtube.com##ytm-pivot-bar-item-renderer:has(.pivot-shorts)

! Hide all videos with the shorts indicator on the thumbnail
m.youtube.com##ytm-video-with-context-renderer:has([data-style="SHORTS"])

! Hide shorts sections
m.youtube.com##ytm-rich-section-renderer:has(.reel-shelf-title-wrapper .yt-core-attributed-string:has-text(/(^| )Shorts( |$)/i))
m.youtube.com##ytm-reel-shelf-renderer.item:has(.reel-shelf-title-wrapper .yt-core-attributed-string:has-text(/(^| )Shorts( |$)/i))

! Hide shorts tab on channel pages
! Old style
m.youtube.com##.single-column-browse-results-tabs>a:has-text(Shorts)
! New style (2023-10)
m.youtube.com##yt-tab-shape:has-text(/^Shorts$/)

! Hide short remixes in video descriptions
m.youtube.com##ytm-reel-shelf-renderer:has(.reel-shelf-title-wrapper .yt-core-attributed-string:has-text(/^Shorts remixing this video$/i))

! Hide shorts category on homepage
m.youtube.com##ytm-chip-cloud-chip-renderer:has(.yt-core-attributed-string:has-text(/^Shorts$/i))
```

### Block zip and mov domains

```
! Block .zip and .mov domains
||zip^
||mov^
```