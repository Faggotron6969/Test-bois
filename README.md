
<!doctype HTML>
<html lang="us">
<link rel="icon" type="image/png" href="image_res/favicon.ico">

    <link rel="image_src" href="http://trainertower.com/damagecalc/image_res/rhydon.png" />
    <html xmlns="http://www.w3.org/1999/xhtml"
    xmlns:og="http://ogp.me/ns#">
    <meta property="og:title" content="Trainer Tower Damage Calculator" />
    <meta property="og:type" content="website" />
    <meta property="og:image" content="http://trainertower.com/damagecalc/image_res/rhydon.png" />

<script>
  (function(i,s,o,g,r,a,m){i['GoogleAnalyticsObject']=r;i[r]=i[r]||function(){
  (i[r].q=i[r].q||[]).push(arguments)},i[r].l=1*new Date();a=s.createElement(o),
  m=s.getElementsByTagName(o)[0];a.async=1;a.src=g;m.parentNode.insertBefore(a,m)
  })(window,document,'script','//www.google-analytics.com/analytics.js','ga');

  ga('create', 'UA-86401070-1', 'auto');
  ga('send', 'pageview');

</script>

<head>
    <meta charset="UTF-8" />
    <title>Pokémon Damage Calculator</title>
    <link href='https://fonts.googleapis.com/css?family=Open+Sans' rel='stylesheet' type='text/css'>
    <link type="text/css" rel="stylesheet" href="script_res/select2.css" />
    <link type="text/css" rel="stylesheet" href="script_res/ap_calc.css" />
    <link type="text/css" rel="stylesheet" href="script_res/nb_calc.css" />
    <link href="https://afeld.github.io/emoji-css/emoji.css" rel="stylesheet">
</head>
<body>
    <div class="header"><div class="wrapper">
            <span class="header-logo"><a href="http://trainertower.com"><img src="image_res/trainertower.png" alt="Trainer Tower" height="50px" /></a></span><span class="nav"><a href="http://trainertower.com">Home</a> | <a href="http://trainertower.com/forums">Forums</a> | <a href="http://play.pokemonshowdown.com/vgc">Showdown</a> | <a href="http://www.trainertower.com/vgc-2018-speed-tiers/">2018 Speed Tiers</a> | <a href="https://github.com/jake-white/VGC-Damage-Calculator">GitHub Page</a> | <a href="https://lilymaniac.github.io/calc/">한국어 계산기 (Korean Version)</a> | <a href="http://trainertower.com/usage-stats">Showdown Stats</a> | <a href="http://www.trainertower.com/WCS-battle-spot-usage/">Battlespot Stats</a> | <a href="http://www.trainertower.com/survivalcalc/">Survival Calc</a></span>
            <div style="clear:both"></div>

    </div></div>
    <div class="wrapper">
        <div>
            <span class="title-text">Malie City Monarchs Calculator - Queen Edition</span>
            <span  class="generations" title="Select the generation.">
                <input class="gen btn-input" type="radio" name="gen" value="1" id="gen1" /><label class="btn btn-small btn-left" for="gen1">RBY</label>
                <input class="gen btn-input" type="radio" name="gen" value="2" id="gen2" /><label class="btn btn-small btn-mid" for="gen2">GSC</label>
                <input class="gen btn-input" type="radio" name="gen" value="3" id="gen3" /><label class="btn btn-small btn-mid" for="gen3">ADV</label>
                <input class="gen btn-input" type="radio" name="gen" value="4" id="gen4" /><label class="btn btn-small btn-mid" for="gen4">DPP</label>
                <input class="gen btn-input" type="radio" name="gen" value="5" id="gen5" /><label class="btn btn-small btn-mid" for="gen5">B/W</label>
                <input class="gen btn-input" type="radio" name="gen" value="6" id="gen6" /><label class="btn btn-small btn-mid" for="gen6">ORAS</label>
                <input class="gen btn-input" type="radio" name="gen" value="7" id="gen7" checked="checked" /><label class="btn btn-small btn-right" for="gen7">USUM</label>
            </span>
        </div>
        <hr />
    <div align="center"><script async src="//pagead2.googlesyndication.com/pagead/js/adsbygoogle.js"></script>
    <!-- Damage Calc Ad -->
    <ins class="adsbygoogle"
         style="display:inline-block;width:728px;height:90px"
         data-ad-client="ca-pub-1513870120798988"
         data-ad-slot="8348790551"></ins>
    <script>
    (adsbygoogle = window.adsbygoogle || []).push({});
    </script>
    </div>
    <p>Ultra Sun & Ultra Moon VGC calculator by Jake White (<a href="https://twitter.com/squirrelboyVGC">@squirrelboyVGC</a>). Submit bug/feature reports/requests through <a href="https://github.com/jake-white/VGC-Damage-Calculator/issues" target="_blank">Github</a> or <a href="http://www.trainertower.com/forums/threads/damage-calculator-bug-reports.62/" target="_blank">this thread</a>, not through Twitter please :)</p>
    <p style="color: #1DA1F2;">#GodSaveTheQueen</p>
    <!-- OLD NUGGETBRIDGE ADS -->
    <!-- TRAINER TOWER ADS GO HERE :) -->
    <!-- <div class="banner"><script async src="http://pagead2.googlesyndication.com/pagead/js/adsbygoogle.js"></script> -->
    <!-- Damage Calc Header -->
    <!-- <ins class="adsbygoogle"
         style="display:inline-block;width:728px;height:90px"
         data-ad-client="ca-pub-2706545500271292"
         data-ad-slot="2267027703"></ins>
    <script>
    (adsbygoogle = window.adsbygoogle || []).push({});
    </script></div> -->
        <div class="move-result-group" title="Select a move to show detailed results.">
            <div class="move-result-subgroup">
                <div class="result-move-header"><span id="resultHeaderL">Pokemon 1's Moves (select one to show detailed results)</span></div>
                <div><input class="result-move btn-input" type="radio" name="resultMove" id="resultMoveL1" checked="checked" /><label class="btn btn-xxxwide btn-top" for="resultMoveL1">Hi Jump Kick</label> <span id="resultDamageL1">??? - ???%</span></div>
                <div><input class="result-move btn-input" type="radio" name="resultMove" id="resultMoveL2" /><label class="btn btn-xxxwide btn-mid" for="resultMoveL2">Falcon Punch</label> <span id="resultDamageL2">??? - ???%</span></div>
                <div><input class="result-move btn-input" type="radio" name="resultMove" id="resultMoveL3" /><label class="btn btn-xxxwide btn-mid" for="resultMoveL3">Suspicious Odor</label> <span id="resultDamageL3">??? - ???%</span></div>
                <div><input class="result-move btn-input" type="radio" name="resultMove" id="resultMoveL4" /><label class="btn btn-xxxwide btn-bottom" for="resultMoveL4">Tombstoner</label> <span id="resultDamageL4">??? - ???%</span></div>
            </div>
            <div class="move-result-subgroup">
                <div class="result-move-header"><span id="resultHeaderR">Pokemon 2's Moves (select one to show detailed results)</span></div>
                <div><input class="result-move btn-input" type="radio" name="resultMove" id="resultMoveR1" /><label class="btn btn-xxxwide btn-top" for="resultMoveR1">Hi Jump Kick</label> <span id="resultDamageR1">??? - ???%</span></div>
                <div><input class="result-move btn-input" type="radio" name="resultMove" id="resultMoveR2" /><label class="btn btn-xxxwide btn-mid" for="resultMoveR2">Falcon Punch</label> <span id="resultDamageR2">??? - ???%</span></div>
                <div><input class="result-move btn-input" type="radio" name="resultMove" id="resultMoveR3" /><label class="btn btn-xxxwide btn-mid" for="resultMoveR3">Suspicious Odor</label> <span id="resultDamageR3">??? - ???%</span></div>
                <div><input class="result-move btn-input" type="radio" name="resultMove" id="resultMoveR4" /><label class="btn btn-xxxwide btn-bottom" for="resultMoveR4">Tombstoner</label> <span id="resultDamageR4">??? - ???%</span></div>
            </div>
        </div>
        <div class="main-result-group">
            <div class="big-text"><span id="mainResult">Loading...</span></div>
            <div class="small-text"><span id="damageValues">(If you see this message for more than a few seconds, try enabling JavaScript. If you have that enabled, try deleting your cookies. Otherwise, I won't be able to help you unless you send a screenshot of your browser console.)</span></div>
        </div>

        <div class="panel poke-info" id="p1">
            <div class="panel-heading"><h4 class="panel-title">Pokémon 1</h4></div>
            <div class="panel-body">
                <input type="text" class="set-selector calc-trigger" />
                <div class="info-group">
                    <div>
                        <label>Type</label>
                        <select class="type1 terrain-trigger calc-trigger"></select>
                        <select class="type2 terrain-trigger calc-trigger"></select>
                    </div>
                    <div class="hide">
                        <label>Forme</label>
                        <select class="forme calc-trigger"></select>
                    </div>
                    <div>
                        <label>Level</label>
                        <input class="level calc-trigger" value="100" />
                    </div>
                    <div class="hide">
                        <label>Weight (kg)</label>
                        <input class="weight calc-trigger" value="10.0" />
                    </div>
                </div>
                <div class="info-group">
                    <table>
                        <tr><th></th><th>Base</th><th class="gen-specific g3 g4 g5 g6 g7 g7">IVs</th><th class="gen-specific g3 g4 g5 g6 g7 g7">EVs</th><th class="gen-specific g1 g2 hide">DVs</th><th></th><th></th></tr>
                        <tr class="hp"><td><label>HP</label></td><td><input class="base calc-trigger" value="100" /></td><td class="gen-specific g3 g4 g5 g6 g7"><input class="ivs calc-trigger" value="31" /></td><td class="gen-specific g3 g4 g5 g6 g7"><input class="evs calc-trigger" type="number" min="0" max="252" step="4" value="0" /></td><td class="gen-specific g1 g2 hide"><input class="dvs calc-trigger" value="15" disabled="disabled" /></td><td><span class="total">341</span></td><td></td></tr>
                        <tr class="at"><td><label>Attack</label></td><td><input class="base calc-trigger" value="100" /></td><td class="gen-specific g3 g4 g5 g6 g7"><input class="ivs calc-trigger" value="31" /></td><td class="gen-specific g3 g4 g5 g6 g7"><input class="evs calc-trigger" type="number" min="0" max="252" step="4" value="0" /></td><td class="gen-specific g1 g2 hide"><input class="dvs calc-trigger" value="15" /></td><td><span class="total">236</span></td><td><select class="boost calc-trigger"><option value="6">+6</option><option value="5">+5</option><option value="4">+4</option><option value="3">+3</option><option value="2">+2</option><option value="1">+1</option><option value="0" selected="selected">--</option><option value="-1">-1</option><option value="-2">-2</option><option value="-3">-3</option><option value="-4">-4</option><option value="-5">-5</option><option value="-6">-6</option></select></td></tr>
                        <tr class="df"><td><label>Defense</label></td><td><input class="base calc-trigger" value="100" /></td><td class="gen-specific g3 g4 g5 g6 g7"><input class="ivs calc-trigger" value="31" /></td><td class="gen-specific g3 g4 g5 g6 g7"><input class="evs calc-trigger" type="number" min="0" max="252" step="4" value="0" /></td><td class="gen-specific g1 g2 hide"><input class="dvs calc-trigger" value="15" /></td><td><span class="total">236</span></td><td><select class="boost calc-trigger"><option value="6">+6</option><option value="5">+5</option><option value="4">+4</option><option value="3">+3</option><option value="2">+2</option><option value="1">+1</option><option value="0" selected="selected">--</option><option value="-1">-1</option><option value="-2">-2</option><option value="-3">-3</option><option value="-4">-4</option><option value="-5">-5</option><option value="-6">-6</option></select></td></tr>
                        <tr class="sa gen-specific g2 g3 g4 g5 g6 g7"><td><label>Sp. Atk</label></td><td><input class="base calc-trigger" value="100" /></td><td class="gen-specific g3 g4 g5 g6 g7"><input class="ivs calc-trigger" value="31" /></td><td class="gen-specific g3 g4 g5 g6 g7"><input class="evs calc-trigger" type="number" min="0" max="252" step="4" value="0" /></td><td class="gen-specific g1 g2 hide"><input class="dvs calc-trigger" value="15" /></td><td><span class="total">236</span></td><td><select class="boost calc-trigger"><option value="6">+6</option><option value="5">+5</option><option value="4">+4</option><option value="3">+3</option><option value="2">+2</option><option value="1">+1</option><option value="0" selected="selected">--</option><option value="-1">-1</option><option value="-2">-2</option><option value="-3">-3</option><option value="-4">-4</option><option value="-5">-5</option><option value="-6">-6</option></select></td></tr>
                        <tr class="sd gen-specific g2 g3 g4 g5 g6 g7"><td><label>Sp. Def</label></td><td><input class="base calc-trigger" value="100" /></td><td class="gen-specific g3 g4 g5 g6 g7"><input class="ivs calc-trigger" value="31" /></td><td class="gen-specific g3 g4 g5 g6 g7"><input class="evs calc-trigger" type="number" min="0" max="252" step="4" value="0" /></td><td class="gen-specific g1 g2 hide"><input class="dvs calc-trigger" value="15" disabled="disabled" /></td><td><span class="total">236</span></td><td><select class="boost calc-trigger"><option value="6">+6</option><option value="5">+5</option><option value="4">+4</option><option value="3">+3</option><option value="2">+2</option><option value="1">+1</option><option value="0" selected="selected">--</option><option value="-1">-1</option><option value="-2">-2</option><option value="-3">-3</option><option value="-4">-4</option><option value="-5">-5</option><option value="-6">-6</option></select></td></tr>
                        <tr class="sl gen-specific g1 hide"><td><label>Special</label></td><td><input class="base calc-trigger" value="100" /></td><td><input class="dvs calc-trigger" value="15" /></td><td><span class="total">236</span></td><td><select class="boost calc-trigger"><option value="6">+6</option><option value="5">+5</option><option value="4">+4</option><option value="3">+3</option><option value="2">+2</option><option value="1">+1</option><option value="0" selected="selected">--</option><option value="-1">-1</option><option value="-2">-2</option><option value="-3">-3</option><option value="-4">-4</option><option value="-5">-5</option><option value="-6">-6</option></select></td></tr>
                        <tr class="sp"><td><label>Speed</label></td><td><input class="base calc-trigger" value="100" /></td><td class="gen-specific g3 g4 g5 g6 g7"><input class="ivs calc-trigger" value="31" /></td><td class="gen-specific g3 g4 g5 g6 g7"><input class="evs calc-trigger" type="number" min="0" max="252" step="4" value="0" /></td><td class="gen-specific g1 g2 hide"><input class="dvs calc-trigger" value="15" /></td><td><span class="total">236</span></td><td><select class="boost calc-trigger"><option value="6">+6</option><option value="5">+5</option><option value="4">+4</option><option value="3">+3</option><option value="2">+2</option><option value="1">+1</option><option value="0" selected="selected">--</option><option value="-1">-1</option><option value="-2">-2</option><option value="-3">-3</option><option value="-4">-4</option><option value="-5">-5</option><option value="-6">-6</option></select></td></tr>
                        <tr><td></td><td></td><td></td><td class='ev-total'>&nbsp;</td><td class='ev-left'>&nbsp;</td><td></td><td></td><td></td></tr>
                    </table>
                </div>
                <div class="info-group info-selectors">
                    <div class="gen-specific g3 g4 g5 g6 g7">
                        <label>Nature</label>
                        <select class="nature calc-trigger"><option value="Adamant">Adamant (+Atk, -SpA)</option><option value="Bashful">Bashful</option><option value="Bold">Bold (+Def, -Atk)</option><option value="Brave">Brave (+Atk, -Spe)</option><option value="Calm">Calm (+SpD, -Atk)</option><option value="Careful">Careful (+SpD, -SpA)</option><option value="Docile">Docile</option><option value="Gentle">Gentle (+SpD, -Def)</option><option value="Hardy" selected="selected">Hardy</option><option value="Hasty">Hasty (+Spe, -Def)</option><option value="Impish">Impish (+Def, -SpA)</option><option value="Jolly">Jolly (+Spe, -SpA)</option><option value="Lax">Lax (+Def, -SpD)</option><option value="Lonely">Lonely (+Atk, -Def)</option><option value="Mild">Mild (+SpA, -Def)</option><option value="Modest">Modest (+SpA, -Atk)</option><option value="Naive">Naive (+Spe, -SpD)</option><option value="Naughty">Naughty (+Atk, -SpD)</option><option value="Quiet">Quiet (+SpA, -Spe)</option><option value="Quirky">Quirky</option><option value="Rash">Rash (+SpA, -SpD)</option><option value="Relaxed">Relaxed (+Def, -Spe)</option><option value="Sassy">Sassy (+SpD, -Spe)</option><option value="Serious">Serious</option><option value="Timid">Timid (+Spe, -Atk)</option></select>
                    </div>
                    <div class="gen-specific g3 g4 g5 g6 g7">
                        <label>Ability</label>
                        <select class="ability terrain-trigger calc-trigger"></select>
                    </div>
                    <div class="gen-specific g2 g3 g4 g5 g6 g7">
                        <label>Item</label>
                        <select class="item terrain-trigger calc-trigger"></select>
                    </div>
                    <div>
                        <label>Status</label>
                        <select class="status calc-trigger"><option value="Healthy">Healthy</option><option value="Poisoned">Poisoned</option><option value="Badly Poisoned">Badly Poisoned</option><option value="Burned">Burned</option><option value="Paralyzed">Paralyzed</option><option value="Asleep">Asleep</option><option value="Frozen">Frozen</option></select>
                        <select class="toxic-counter calc-trigger hide"><option value="1">1/16</option><option value="2">2/16</option><option value="3">3/16</option><option value="4">4/16</option><option value="5">5/16</option><option value="6">6/16</option><option value="7">7/16</option><option value="8">8/16</option><option value="9">9/16</option><option value="10">10/16</option><option value="11">11/16</option><option value="12">12/16</option><option value="13">13/16</option><option value="14">14/16</option><option value="15">15/16</option></select>
                    </div>
                </div>
                <div class="info-group">
                    <label>Current HP</label>
                    <input class="current-hp calc-trigger" value="341" />/<span class="max-hp">341</span> (<input class="percent-hp calc-trigger" value="100" />%)
                </div>
                <div class="move1">
                    <select class="move-selector calc-trigger small-select"></select>
                    <input class="move-bp calc-trigger" value="50" />
                    <select class="move-type calc-trigger"></select>
                    <select class="move-cat calc-trigger gen-specific g4 g5 g6 g7"><option value="Physical">Physical</option><option value="Special">Special</option></select>
                    <input class="move-crit calc-trigger btn-input" type="checkbox" id="critL1" /><label class="btn crit-btn" for="critL1" title="Force this attack to be a critical hit?">Crit</label>
                    <input class="move-z calc-trigger btn-input" type="checkbox" id="zL1" /><label class="btn x-btn" for="zL1" title="Use the corresponding Z-Move?">Z-Move</label>
                    <select class="move-hits calc-trigger hide"><option value="2">2 hits</option><option value="3">3 hits</option><option value="4">4 hits</option><option value="5">5 hits</option></select>
                </div>
                <div class="move2">
                    <select class="move-selector calc-trigger small-select"></select>
                    <input class="move-bp calc-trigger" value="0" />
                    <select class="move-type calc-trigger"></select>
                    <select class="move-cat calc-trigger gen-specific g4 g5 g6 g7"><option value="Physical">Physical</option><option value="Special">Special</option></select>
                    <input class="move-crit calc-trigger btn-input" type="checkbox" id="critL2" /><label class="btn crit-btn" for="critL2" title="Force this attack to be a critical hit?">Crit</label>
                    <input class="move-z calc-trigger btn-input" type="checkbox" id="zL2" /><label class="btn x-btn" for="zL2" title="Use the corresponding Z-Move?">Z-Move</label>
                    <select class="move-hits calc-trigger hide"><option value="2">2 hits</option><option value="3">3 hits</option><option value="4">4 hits</option><option value="5">5 hits</option></select>
                </div>
                <div class="move3">
                    <select class="move-selector calc-trigger small-select"></select>
                    <input class="move-bp calc-trigger" value="0" />
                    <select class="move-type calc-trigger"></select>
                    <select class="move-cat calc-trigger gen-specific g4 g5 g6 g7"><option value="Physical">Physical</option><option value="Special">Special</option></select>
                    <input class="move-crit calc-trigger btn-input" type="checkbox" id="critL3" /><label class="btn crit-btn" for="critL3" title="Force this attack to be a critical hit?">Crit</label>
                    <input class="move-z calc-trigger btn-input" type="checkbox" id="zL3" /><label class="btn x-btn" for="zL3" title="Use the corresponding Z-Move?">Z-Move</label>
                    <select class="move-hits calc-trigger hide"><option value="2">2 hits</option><option value="3">3 hits</option><option value="4">4 hits</option><option value="5">5 hits</option></select>
                </div>
                <div class="move4">
                    <select class="move-selector calc-trigger small-select"></select>
                    <input class="move-bp calc-trigger" value="0" />
                    <select class="move-type calc-trigger"></select>
                    <select class="move-cat calc-trigger gen-specific g4 g5 g6 g7"><option value="Physical">Physical</option><option value="Special">Special</option></select>
                    <input class="move-crit calc-trigger btn-input" type="checkbox" id="critL4" /><label class="btn crit-btn" for="critL4" title="Force this attack to be a critical hit?">Crit</label>
                    <input class="move-z calc-trigger btn-input" type="checkbox" id="zL4" /><label class="btn x-btn" for="zL4" title="Use the corresponding Z-Move?">Z-Move</label>
                    <select class="move-hits calc-trigger hide"><option value="2">2 hits</option><option value="3">3 hits</option><option value="4">4 hits</option><option value="5">5 hits</option></select>
                </div>

            </div>
        </div>

        <div class="panel field-info">
            <div class="panel-heading">
                <h4 class="panel-title">Field
                    <div id = "autolevel">Auto-Level to:
                        <div class="onoffswitch" style="margin-left: 1em">
                                <input type="checkbox" name="onoffswitch" class="onoffswitch-checkbox" id="douswitch" checked>
                                <label class="onoffswitch-label" for="douswitch">
                                <span class="onoffswitch-inner"></span>
                                <span class="onoffswitch-switch"></span>
                            </label>
                        </div>
                    </div>
                </h4>
            </div>
            <div class="panel-body">
                <img id="malie" align = "center" src="image_res/malie.png" alt="Mimikyu da yo" style= "display: block;  margin: 0 auto;">
                <div class="gen-specific g3 g4 g5 g6 g7" style="width: 10.6em; margin: 0 auto 5px;" title="Select the battle format.">
                    <input class="btn-input calc-trigger" type="radio" name="format" value="Singles" id="singles" checked="checked" /><label class="btn btn-left" for="singles">Singles</label>
                    <input class="btn-input calc-trigger" type="radio" name="format" value="Doubles" id="doubles" /><label class="btn btn-right" for="doubles">Doubles</label>
                </div>
                <div class="gen-specific g6 g7" style="width: 22.0em; margin: 5px auto;" title="Select the current terrain.">
                    <input class="btn-input terrain-trigger calc-trigger" type="radio" name="terrain" value="" id="noterrain" checked="checked" /><label class="btn btn-small btn-left" for="noterrain">None</label>
                    <input class="btn-input terrain-trigger calc-trigger" type="radio" name="terrain" value="Electric" id="electric" /><label class="btn btn-small btn-mid" for="electric">Electric</label>
                    <input class="btn-input terrain-trigger calc-trigger" type="radio" name="terrain" value="Grassy" id="grassy" /><label class="btn btn-small btn-mid" for="grassy">Grassy</label>
                    <input class="btn-input terrain-trigger calc-trigger" type="radio" name="terrain" value="Misty" id="misty" /><label class="btn btn-small btn-mid" for="misty">Misty</label>
                    <input class="btn-input terrain-trigger calc-trigger" type="radio" name="terrain" value="Psychic" id="psychic" /><label class="btn btn-small btn-right" for="psychic">Psychic</label>
                </div>
                <hr class="gen-specific g6 g7 g7" />
                <div class="gen-specific g3 g4 g5 g6 g7 g7" style="width: 22.2em; margin: 5px auto;" title="Select the current weather condition.">
                    <input class="btn-input calc-trigger" type="radio" name="weather" value="" id="clear" checked="checked" /><label class="btn btn-small btn-left" for="clear">None</label>
                    <input class="btn-input calc-trigger" type="radio" name="weather" value="Sun" id="sun" /><label class="btn btn-small btn-mid" for="sun">Sun</label>
                    <input class="btn-input calc-trigger" type="radio" name="weather" value="Rain" id="rain" /><label class="btn btn-small btn-mid" for="rain">Rain</label>
                    <input class="btn-input calc-trigger" type="radio" name="weather" value="Sand" id="sand" /><label class="btn btn-small btn-mid" for="sand">Sand</label>
                    <input class="btn-input calc-trigger" type="radio" name="weather" value="Hail" id="hail" /><label class="btn btn-small btn-right" for="hail">Hail</label>
                </div>
                <div class="gen-specific g6 g7 g7" style="width: 21.1em; margin: 5px auto;" title="Select the current weather condition.">
                    <input class="btn-input calc-trigger" type="radio" name="weather" value="Harsh Sun" id="harsh-sun"/><label class="btn btn-wide btn-left" for="harsh-sun">Harsh Sun</label>
                    <input class="btn-input calc-trigger" type="radio" name="weather" value="Heavy Rain" id="heavy-rain"/><label class="btn btn-wide btn-mid" for="heavy-rain">Heavy Rain</label>
                    <input class="btn-input calc-trigger" type="radio" name="weather" value="Strong Winds" id="strong-winds"/><label class="btn btn-xwide btn-right" for="strong-winds">Strong Winds</label>
                </div>
                <div class="gen-specific g2 hide" style="width: 17.8em; margin: 0 auto 5px;" title="Select the current weather condition.">
                    <input class="btn-input calc-trigger" type="radio" name="gscWeather" value="" id="gscClear" checked="checked" /><label class="btn btn-small btn-left" for="gscClear">None</label>
                    <input class="btn-input calc-trigger" type="radio" name="gscWeather" value="Sun" id="gscSun" /><label class="btn btn-small btn-mid" for="gscSun">Sun</label>
                    <input class="btn-input calc-trigger" type="radio" name="gscWeather" value="Rain" id="gscRain" /><label class="btn btn-small btn-mid" for="gscRain">Rain</label>
                    <input class="btn-input calc-trigger" type="radio" name="gscWeather" value="Sand" id="gscSand" /><label class="btn btn-small btn-right" for="gscSand">Sand</label>
                </div>
                <div class="gen-specific g6 g7 g7" style="width: 21.1em; margin: 5px auto;" title="Select the current radiating aura.">
                <input class="btn-input calc-trigger" type="checkbox" name="aura" value="Aura Break" id="aura-break"/><label class="btn btn-wide btn-left" for="aura-break">Aura Break</label>
                <input class="btn-input calc-trigger" type="checkbox" name="aura" value="Fairy Aura" id="fairy-aura"/><label class="btn btn-wide btn-mid" for="fairy-aura">Fairy Aura</label>
                <input class="btn-input calc-trigger" type="checkbox" name="aura" value="Dark Aura" id="dark-aura"/><label class="btn btn-wide btn-right" for="dark-aura">Dark Aura</label>
                </div>
                <div class="gen-specific g4 g5 g6 g7 g7" style="width: 5.3em; margin: 5px auto;" title="Is gravity in effect?">
                    <input class="btn-input calc-trigger" type="checkbox" id="gravity" /><label class="btn" for="gravity">Gravity</label>
                </div>
                <hr class="gen-specific g2 g3 g4 g5 g6 g7 g7" />

                <div class="btn-group gen-specific g7">
                    <div class="left" title="Is this Pokemon protecting?">
                        <input class="btn-input calc-trigger" type="checkbox" id="protectL" /><label class="btn btn-xwide" for="protectL">Protect</label>
                    </div>
                    <div class="right" title="Is this Pokemon protecting?">
                        <input class="btn-input calc-trigger" type="checkbox" id="protectR" /><label class="btn btn-xwide" for="protectR">Protect</label>
                    </div>
                </div>
                <div class="btn-group gen-specific g4 g5 g6 g7 g7">
                    <div class="left" title="Is Stealth Rock affecting this side of the field?">
                        <input class="btn-input calc-trigger" type="checkbox" id="srL" /><label class="btn btn-xwide" for="srL">Stealth Rock</label>
                    </div>
                    <div class="right" title="Is Stealth Rock affecting this side of the field?">
                        <input class="btn-input calc-trigger" type="checkbox" id="srR" /><label class="btn btn-xwide" for="srR">Stealth Rock</label>
                    </div>
                </div>
                <div class="btn-group gen-specific g3 g4 g5 g6 g7 g7">
                    <div class="left" title="Are there Spikes on this side of the field?">
                        <input class="btn-input calc-trigger" type="radio" name="spikesL" value="0" id="spikesL0" checked="checked" /><label class="btn btn-xsmall btn-left" for="spikesL0">0</label>
                        <input class="btn-input calc-trigger" type="radio" name="spikesL" value="1" id="spikesL1" /><label class="btn btn-xsmall btn-mid" for="spikesL1">1</label>
                        <input class="btn-input calc-trigger" type="radio" name="spikesL" value="2" id="spikesL2" /><label class="btn btn-xsmall btn-mid" for="spikesL2">2</label>
                        <input class="btn-input calc-trigger" type="radio" name="spikesL" value="3" id="spikesL3" /><label class="btn btn-wide btn-right" for="spikesL3">3 Spikes</label>
                    </div>
                    <div class="right" title="Are there Spikes on this side of the field?">
                        <input class="btn-input calc-trigger" type="radio" name="spikesR" value="0" id="spikesR0" checked="checked" /><label class="btn btn-xsmall btn-left" for="spikesR0">0</label>
                        <input class="btn-input calc-trigger" type="radio" name="spikesR" value="1" id="spikesR1" /><label class="btn btn-xsmall btn-mid" for="spikesR1">1</label>
                        <input class="btn-input calc-trigger" type="radio" name="spikesR" value="2" id="spikesR2" /><label class="btn btn-xsmall btn-mid" for="spikesR2">2</label>
                        <input class="btn-input calc-trigger" type="radio" name="spikesR" value="3" id="spikesR3" /><label class="btn btn-wide btn-right" for="spikesR3">3 Spikes</label>
                    </div>
                </div>
                <div class="btn-group gen-specific g2">
                    <div class="left" title="Are there Spikes on this side of the field?">
                        <input class="btn-input calc-trigger" type="checkbox" id="gscSpikesL" /><label class="btn" for="gscSpikesL">Spikes</label>
                    </div>
                    <div class="right" title="Are there Spikes on this side of the field?">
                        <input class="btn-input calc-trigger" type="checkbox" id="gscSpikesR" /><label class="btn" for="gscSpikesR">Spikes</label>
                    </div>
                </div>
                <div class="btn-group">
                    <div class="left" title="Is this Pokemon protected by Reflect and/or Light Screen?">
                        <input class="btn-input calc-trigger" type="checkbox" id="reflectL" /><label class="btn btn-left" for="reflectL">Reflect</label>
                        <input class="btn-input calc-trigger" type="checkbox" id="lightScreenL" /><label class="btn btn-xwide btn-right" for="lightScreenL">Light Screen</label>
                    </div>
                    <div class="right" title="Is this Pokemon protected by Reflect and/or Light Screen?">
                        <input class="btn-input calc-trigger" type="checkbox" id="reflectR" /><label class="btn btn-left" for="reflectR">Reflect</label>
                        <input class="btn-input calc-trigger" type="checkbox" id="lightScreenR" /><label class="btn btn-xwide btn-right" for="lightScreenR">Light Screen</label>
                    </div>
                </div>
                <div class="btn-group gen-specific g2 g3 g4 g5 g6 g7 g7">
                    <div class="left" title="Has this Pokemon been revealed with Foresight or Odor Sleuth?">
                        <input class="btn-input calc-trigger" type="checkbox" id="foresightL" /><label class="btn btn-wide" for="foresightL">Foresight</label>
                    </div>
                    <div class="right" title="Has this Pokemon been revealed with Foresight or Odor Sleuth?">
                        <input class="btn-input calc-trigger" type="checkbox" id="foresightR" /><label class="btn btn-wide" for="foresightR">Foresight</label>
                    </div>
                </div>
                <div class="btn-group gen-specific g3 g4 g5 g6 g7 g7">
                    <div class="left" title="Has this Pokemon's power been boosted by an ally's Helping Hand?">
                        <input class="btn-input calc-trigger" type="checkbox" id="helpingHandL" /><label class="btn btn-xxwide" for="helpingHandL">Helping Hand</label>
                    </div>
                    <div class="right" title="Has this Pokemon's power been boosted by an ally's Helping Hand?">
                        <input class="btn-input calc-trigger" type="checkbox" id="helpingHandR" /><label class="btn btn-xxwide" for="helpingHandR">Helping Hand</label>
                    </div>
                </div>
                <div class="btn-group gen-specific g7">
                    <div class="left" title="Has this Pokemon's power been boosted by an ally's Battery?">
                        <input class="btn-input calc-trigger" type="checkbox" id="batteryL" /><label class="btn btn-xxwide" for="batteryL">Battery</label>
                    </div>
                    <div class="right" title="Has this Pokemon's power been boosted by an ally's Battery?">
                        <input class="btn-input calc-trigger" type="checkbox" id="batteryR" /><label class="btn btn-xxwide" for="batteryR">Battery</label>
                    </div>
                </div>
                <div class="btn-group gen-specific g5 g6 g7 g7">
                    <div class="left" title="Is this Pokemon protected by an ally's Friend Guard?">
                        <input class="btn-input calc-trigger" type="checkbox" id="friendGuardL" /><label class="btn btn-xxwide" for="friendGuardL">Friend Guard</label>
                    </div>
                    <div class="right" title="Is this Pokemon protected by an ally's Friend Guard?">
                        <input class="btn-input calc-trigger" type="checkbox" id="friendGuardR" /><label class="btn btn-xxwide" for="friendGuardR">Friend Guard</label>
                    </div>
                </div>

                <div class="btn-group gen-specific g7">
                    <div class="left" title="Has this Pokemon used Clangorous Soulblaze?">
                        <input class="btn-input calc-trigger" type="checkbox" id="clangL" /><label class="btn btn-xwide" for="clangL"><img src="image_res/784.png"><br>Clangorous Soulblaze</label>
                    </div>
                    <div class="right" title="Has this Pokemon used Clangorous Soulblaze?">
                        <input class="btn-input calc-trigger" type="checkbox" id="clangR" /><label class="btn btn-xwide" for="clangR"><img src="image_res/784.png"><br>Clangorous Soulblaze</label>
                    </div>
                </div>

                <div class="btn-group gen-specific g7">
                    <div class="left" title="Has this Pokemon used Extreme Evoboost?">
                        <input class="btn-input calc-trigger" type="checkbox" id="evoL" /><label class="btn btn-xwide" for="evoL"><img src="image_res/133.png"><br>Extreme Evoboost</label>
                    </div>
                    <div class="right" title="Has this Pokemon used Extreme Evoboost?">
                        <input class="btn-input calc-trigger" type="checkbox" id="evoR" /><label class="btn btn-xwide" for="evoR"><img src="image_res/133.png"><br>Extreme Evoboost</label>
                    </div>
                </div>

                <!--squirrelboy1225's HTML additions are right here-->

                <!--...two years later, my HTML additions are fucking everywhere. they spread like cancer-->
                <p>Please enter your custom set here.</p>
                Spread Name: <input type = "text" id = "spreadName" style = "width: 60%" value = "My Custom Set">
                <br>
                <textarea rows="9" cols="40" id = "customMon"></textarea>
                <br>
                <script type="text/javascript" src="script_res/setdex_custom.js"></script>
                <button type = "button" onclick = "savecustom()">Save</button> <button type = "button" onclick = "deletecustom()">Delete Custom Sets</button>
                <p>You may need to refresh the page after deleting your custom sets.  If you encounter a bug, please try deleting your cookies or reporting it!</p>
            </div>
        </div>
        <div class="panel poke-info" id="p2">
            <div class="panel-heading"><h4 class="panel-title">Pokémon 2</h4></div>
            <div class="panel-body">
                <input type="text" class="set-selector calc-trigger" />
                <div class="info-group">
                    <div>
                        <label>Type</label>
                        <select class="type1 terrain-trigger calc-trigger"></select>
                        <select class="type2 terrain-trigger calc-trigger"></select>
                    </div>
                    <div class="hide">
                        <label>Forme</label>
                        <select class="forme calc-trigger"></select>
                    </div>
                    <div>
                        <label>Level</label>
                        <input class="level calc-trigger" value="100" />
                    </div>
                    <div class="hide">
                        <label>Weight (kg)</label>
                        <input class="weight calc-trigger" value="10.0" />
                    </div>
                </div>
                <div class="info-group">
                    <table>
                        <tr><th></th><th>Base</th><th class="gen-specific g3 g4 g5 g6 g7">IVs</th><th class="gen-specific g3 g4 g5 g6 g7">EVs</th><th class="gen-specific g1 g2 hide">DVs</th><th></th><th></th></tr>
                        <tr class="hp"><td><label>HP</label></td><td><input class="base calc-trigger" value="100" /></td><td class="gen-specific g3 g4 g5 g6 g7"><input class="ivs calc-trigger" value="31" /></td><td class="gen-specific g3 g4 g5 g6 g7"><input class="evs calc-trigger" type="number" min="0" max="252" step="4" value="0" /></td><td class="gen-specific g1 g2 hide"><input class="dvs calc-trigger" value="15" disabled="disabled" /></td><td><span class="total">341</span></td><td></td></tr>
                        <tr class="at"><td><label>Attack</label></td><td><input class="base calc-trigger" value="100" /></td><td class="gen-specific g3 g4 g5 g6 g7"><input class="ivs calc-trigger" value="31" /></td><td class="gen-specific g3 g4 g5 g6 g7"><input class="evs calc-trigger" type="number" min="0" max="252" step="4" value="0" /></td><td class="gen-specific g1 g2 hide"><input class="dvs calc-trigger" value="15" /></td><td><span class="total">236</span></td><td><select class="boost calc-trigger"><option value="6">+6</option><option value="5">+5</option><option value="4">+4</option><option value="3">+3</option><option value="2">+2</option><option value="1">+1</option><option value="0" selected="selected">--</option><option value="-1">-1</option><option value="-2">-2</option><option value="-3">-3</option><option value="-4">-4</option><option value="-5">-5</option><option value="-6">-6</option></select></td></tr>
                        <tr class="df"><td><label>Defense</label></td><td><input class="base calc-trigger" value="100" /></td><td class="gen-specific g3 g4 g5 g6 g7"><input class="ivs calc-trigger" value="31" /></td><td class="gen-specific g3 g4 g5 g6 g7"><input class="evs calc-trigger" type="number" min="0" max="252" step="4" value="0" /></td><td class="gen-specific g1 g2 hide"><input class="dvs calc-trigger" value="15" /></td><td><span class="total">236</span></td><td><select class="boost calc-trigger"><option value="6">+6</option><option value="5">+5</option><option value="4">+4</option><option value="3">+3</option><option value="2">+2</option><option value="1">+1</option><option value="0" selected="selected">--</option><option value="-1">-1</option><option value="-2">-2</option><option value="-3">-3</option><option value="-4">-4</option><option value="-5">-5</option><option value="-6">-6</option></select></td></tr>
                        <tr class="sa gen-specific g2 g3 g4 g5 g6 g7"><td><label>Sp. Atk</label></td><td><input class="base calc-trigger" value="100" /></td><td class="gen-specific g3 g4 g5 g6 g7"><input class="ivs calc-trigger" value="31" /></td><td class="gen-specific g3 g4 g5 g6 g7"><input class="evs calc-trigger" type="number" min="0" max="252" step="4" value="0" /></td><td class="gen-specific g1 g2 hide"><input class="dvs calc-trigger" value="15" /></td><td><span class="total">236</span></td><td><select class="boost calc-trigger"><option value="6">+6</option><option value="5">+5</option><option value="4">+4</option><option value="3">+3</option><option value="2">+2</option><option value="1">+1</option><option value="0" selected="selected">--</option><option value="-1">-1</option><option value="-2">-2</option><option value="-3">-3</option><option value="-4">-4</option><option value="-5">-5</option><option value="-6">-6</option></select></td></tr>
                        <tr class="sd gen-specific g2 g3 g4 g5 g6 g7"><td><label>Sp. Def</label></td><td><input class="base calc-trigger" value="100" /></td><td class="gen-specific g3 g4 g5 g6 g7"><input class="ivs calc-trigger" value="31" /></td><td class="gen-specific g3 g4 g5 g6 g7"><input class="evs calc-trigger" type="number" min="0" max="252" step="4" value="0" /></td><td class="gen-specific g1 g2 hide"><input class="dvs calc-trigger" value="15" disabled="disabled" /></td><td><span class="total">236</span></td><td><select class="boost calc-trigger"><option value="6">+6</option><option value="5">+5</option><option value="4">+4</option><option value="3">+3</option><option value="2">+2</option><option value="1">+1</option><option value="0" selected="selected">--</option><option value="-1">-1</option><option value="-2">-2</option><option value="-3">-3</option><option value="-4">-4</option><option value="-5">-5</option><option value="-6">-6</option></select></td></tr>
                        <tr class="sl gen-specific g1 hide"><td><label>Special</label></td><td><input class="base calc-trigger" value="100" /></td><td><input class="dvs calc-trigger" value="15" /></td><td><span class="total">236</span></td><td><select class="boost calc-trigger"><option value="6">+6</option><option value="5">+5</option><option value="4">+4</option><option value="3">+3</option><option value="2">+2</option><option value="1">+1</option><option value="0" selected="selected">--</option><option value="-1">-1</option><option value="-2">-2</option><option value="-3">-3</option><option value="-4">-4</option><option value="-5">-5</option><option value="-6">-6</option></select></td></tr>
                        <tr class="sp"><td><label>Speed</label></td><td><input class="base calc-trigger" value="100" /></td><td class="gen-specific g3 g4 g5 g6 g7"><input class="ivs calc-trigger" value="31" /></td><td class="gen-specific g3 g4 g5 g6 g7"><input class="evs calc-trigger" type="number" min="0" max="252" step="4" value="0" /></td><td class="gen-specific g1 g2 hide"><input class="dvs calc-trigger" value="15" /></td><td><span class="total">236</span></td><td><select class="boost calc-trigger"><option value="6">+6</option><option value="5">+5</option><option value="4">+4</option><option value="3">+3</option><option value="2">+2</option><option value="1">+1</option><option value="0" selected="selected">--</option><option value="-1">-1</option><option value="-2">-2</option><option value="-3">-3</option><option value="-4">-4</option><option value="-5">-5</option><option value="-6">-6</option></select></td></tr>
                        <tr><td></td><td></td><td></td><td class='ev-total'>&nbsp;</td><td class='ev-left'>&nbsp;</td><td></td><td></td><td></td></tr>
                    </table>
                </div>
                <div class="info-group info-selectors">
                    <div class="gen-specific g3 g4 g5 g6 g7">
                        <label>Nature</label>
                        <select class="nature calc-trigger"><option value="Adamant">Adamant (+Atk, -SpA)</option><option value="Bashful">Bashful</option><option value="Bold">Bold (+Def, -Atk)</option><option value="Brave">Brave (+Atk, -Spe)</option><option value="Calm">Calm (+SpD, -Atk)</option><option value="Careful">Careful (+SpD, -SpA)</option><option value="Docile">Docile</option><option value="Gentle">Gentle (+SpD, -Def)</option><option value="Hardy" selected="selected">Hardy</option><option value="Hasty">Hasty (+Spe, -Def)</option><option value="Impish">Impish (+Def, -SpA)</option><option value="Jolly">Jolly (+Spe, -SpA)</option><option value="Lax">Lax (+Def, -SpD)</option><option value="Lonely">Lonely (+Atk, -Def)</option><option value="Mild">Mild (+SpA, -Def)</option><option value="Modest">Modest (+SpA, -Atk)</option><option value="Naive">Naive (+Spe, -SpD)</option><option value="Naughty">Naughty (+Atk, -SpD)</option><option value="Quiet">Quiet (+SpA, -Spe)</option><option value="Quirky">Quirky</option><option value="Rash">Rash (+SpA, -SpD)</option><option value="Relaxed">Relaxed (+Def, -Spe)</option><option value="Sassy">Sassy (+SpD, -Spe)</option><option value="Serious">Serious</option><option value="Timid">Timid (+Spe, -Atk)</option></select>
                    </div>
                    <div class="gen-specific g3 g4 g5 g6 g7">
                        <label>Ability</label>
                        <select class="ability terrain-trigger calc-trigger"></select>
                    </div>
                    <div class="gen-specific g2 g3 g4 g5 g6 g7">
                        <label>Item</label>
                        <select class="item terrain-trigger calc-trigger"></select>
                    </div>
                    <div>
                        <label>Status</label>
                        <select class="status calc-trigger"><option value="Healthy">Healthy</option><option value="Poisoned">Poisoned</option><option value="Badly Poisoned">Badly Poisoned</option><option value="Burned">Burned</option><option value="Paralyzed">Paralyzed</option><option value="Asleep">Asleep</option><option value="Frozen">Frozen</option></select>
                        <select class="toxic-counter calc-trigger hide"><option value="1">1/16</option><option value="2">2/16</option><option value="3">3/16</option><option value="4">4/16</option><option value="5">5/16</option><option value="6">6/16</option><option value="7">7/16</option><option value="8">8/16</option><option value="9">9/16</option><option value="10">10/16</option><option value="11">11/16</option><option value="12">12/16</option><option value="13">13/16</option><option value="14">14/16</option><option value="15">15/16</option></select>
                    </div>
                </div>
                <div class="info-group">
                    <label>Current HP</label>
                    <input class="current-hp calc-trigger" value="341" />/<span class="max-hp">341</span> (<input class="percent-hp calc-trigger" value="100" />%)
                </div>
                <div class="move1">
                    <select class="move-selector calc-trigger small-select"></select>
                    <input class="move-bp calc-trigger" value="50" />
                    <select class="move-type calc-trigger"></select>
                    <select class="move-cat calc-trigger gen-specific g4 g5 g6 g7"><option value="Physical">Physical</option><option value="Special">Special</option></select>
                    <input class="move-crit calc-trigger btn-input" type="checkbox" id="critR1" /><label class="btn crit-btn" for="critR1" title="Force this attack to be a critical hit?">Crit</label>
                    <input class="move-z calc-trigger btn-input" type="checkbox" id="zR1" /><label class="btn x-btn" for="zR1" title="Use the corresponding Z-Move?">Z-Move</label>
                    <select class="move-hits calc-trigger hide"><option value="2">2 hits</option><option value="3">3 hits</option><option value="4">4 hits</option><option value="5">5 hits</option></select>
                </div>
                <div class="move2">
                    <select class="move-selector calc-trigger small-select"></select>
                    <input class="move-bp calc-trigger" value="0" />
                    <select class="move-type calc-trigger"></select>
                    <select class="move-cat calc-trigger gen-specific g4 g5 g6 g7"><option value="Physical">Physical</option><option value="Special">Special</option></select>
                    <input class="move-crit calc-trigger btn-input" type="checkbox" id="critR2" /><label class="btn crit-btn" for="critR2" title="Force this attack to be a critical hit?">Crit</label>
                    <input class="move-z calc-trigger btn-input" type="checkbox" id="zR2" /><label class="btn x-btn" for="zR2" title="Use the corresponding Z-Move?">Z-Move</label>
                    <select class="move-hits calc-trigger hide"><option value="2">2 hits</option><option value="3">3 hits</option><option value="4">4 hits</option><option value="5">5 hits</option></select>
                </div>
                <div class="move3">
                    <select class="move-selector calc-trigger small-select"></select>
                    <input class="move-bp calc-trigger" value="0" />
                    <select class="move-type calc-trigger"></select>
                    <select class="move-cat calc-trigger gen-specific g4 g5 g6 g7"><option value="Physical">Physical</option><option value="Special">Special</option></select>
                    <input class="move-crit calc-trigger btn-input" type="checkbox" id="critR3" /><label class="btn crit-btn" for="critR3" title="Force this attack to be a critical hit?">Crit</label>
                    <input class="move-z calc-trigger btn-input" type="checkbox" id="zR3" /><label class="btn x-btn" for="zR3" title="Use the corresponding Z-Move?">Z-Move</label>
                    <select class="move-hits calc-trigger hide"><option value="2">2 hits</option><option value="3">3 hits</option><option value="4">4 hits</option><option value="5">5 hits</option></select>
                </div>
                <div class="move4">
                    <select class="move-selector calc-trigger small-select"></select>
                    <input class="move-bp calc-trigger" value="0" />
                    <select class="move-type calc-trigger"></select>
                    <select class="move-cat calc-trigger gen-specific g4 g5 g6 g7"><option value="Physical">Physical</option><option value="Special">Special</option></select>
                    <input class="move-crit calc-trigger btn-input" type="checkbox" id="critR4" /><label class="btn crit-btn" for="critR4" title="Force this attack to be a critical hit?">Crit</label>
                    <input class="move-z calc-trigger btn-input" type="checkbox" id="zR4" /><label class="btn x-btn" for="zR4" title="Use the corresponding Z-Move?">Z-Move</label>
                    <select class="move-hits calc-trigger hide"><option value="2">2 hits</option><option value="3">3 hits</option><option value="4">4 hits</option><option value="5">5 hits</option></select>
                </div>
            </div>
        </div>
        <div class="footer">
            <p><em>This calculator is based on the work of Honko, gamut, and Zarel. It was optimized for players in the Pokémon Championship Series by Tapin, Firestorm, and squirrelboy1225. Huge thanks to NuggetBridge for hosting this calculator in the past.</em></p></div>
    </div>
    </body>


    <script src="jquery-3.1.1.min.js"></script>
    <script type="text/javascript" src="script_res/select2.min.js"></script>
    <script type="text/javascript" src="script_res/pokedex.js"></script>
    <script type="text/javascript" src="script_res/setdex_showdown.js"></script>
    <script type="text/javascript" src="script_res/setdex_globalLink.js"></script>
    <script type="text/javascript" src="script_res/setdex_nuggetBridge.js"></script>
    <script type="text/javascript" src="script_res/setdex_tt2017.js" id = "TTScript"></script>
    <script type="text/javascript" src="script_res/setdex_tt2018.js" id = "TTScript"></script>
    <script type="text/javascript" src="script_res/setdex_smogon.js" id = "SmogScript"></script>
    <script type="text/javascript" src="script_res/setdex_xy.js" id = "XYScript"></script>
    <script type="text/javascript" src="script_res/setdex_sm.js" id = "SMScript"></script>
    <script type="text/javascript" src="script_res/setdex_bw.js"></script>
    <script type="text/javascript" src="script_res/setdex_dpp.js"></script>
    <script type="text/javascript" src="script_res/setdex_rse.js"></script>
    <script type="text/javascript" src="script_res/setdex_gsc.js"></script>
    <script type="text/javascript" src="script_res/setdex_rby.js"></script>
    <script type="text/javascript" src="script_res/stat_data.js"></script>
    <script type="text/javascript" src="script_res/type_data.js"></script>
    <script type="text/javascript" src="script_res/nature_data.js"></script>
    <script type="text/javascript" src="script_res/ability_data.js"></script>
    <script type="text/javascript" src="script_res/item_data.js"></script>
    <script type="text/javascript" src="script_res/move_data.js"></script>
    <script type="text/javascript" src="script_res/ap_calc.js"></script>
    <script type="text/javascript" src="script_res/damage.js"></script>
    <script type="text/javascript" src="script_res/damage_dpp.js"></script>
    <script type="text/javascript" src="script_res/damage_rse.js"></script>
    <script type="text/javascript" src="script_res/damage_gsc.js"></script>
    <script type="text/javascript" src="script_res/damage_rby.js"></script>
    <script type="text/javascript" src="script_res/ko_chance.js"></script>
<script type="text/javascript" src="script_res/statuscalc.js"></script>
</html>
