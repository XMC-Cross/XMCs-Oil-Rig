# XMCs-Oil-Rig
Contains all files necessary to have a lootable Oil Rig near Chernogorsk and Shipwreck near Skalisty Island in DayZ!
Before you start changing your server, please make a backup of your server files for any problems that may occur.

These changes DO NOT represent DayZ as it is not an Official Location

First thing is to stop the server [You must stop the server if you plan on using the areaflags.map file]

Wait about 5 minutes for your server to stop, once 5 minutes have gone by, upload the areaflags.map under dayzoffline.chernarusplus (it will override the vanilla one)
This may take awhile, depending on upload speed.
While waiting...
In your file editor (I suggest Visual Studio Code if you don't have one)

Make a new in mapgroupprotto entry - These are not in DayZ vanilla files, they won't spawn loot if you don't add them

		<group name="StaticObj_Wreck_Mi8" lootmax="5">
				<usage name="Military" />
				<container name="lootShelves">
					<category name="tools" />
					<category name="containers" />
					<category name="food" />
					<tag name="shelves" />
					<point pos="-6.850625 -1.421773 -0.344947" range="0.1" height="0.2" /> 
					<point pos="-5.945957 -1.428432 -0.428892" range="0.1" height="0.2" /> 
					<point pos="-4.351717 -1.458216 -0.654538" range="0.1" height="0.2" /> 
					<point pos="-3.668689 -1.460896 -0.707812" range="0.1" height="0.2" /> 
					<point pos="-2.788545 -1.477059 -0.737154" range="0.1" height="0.2" /> 
					<point pos="-2.747982 -1.500877 -2.690142" range="0.1" height="0.2" /> 
				</container>
				<container name="lootFloor">
					<category name="tools" />
					<category name="clothes" />
					<category name="containers" />
					<tag name="floor" />
					<point pos="-7.730903 -1.702977 -1.841105" range="0.7" height="1" /> 
					<point pos="-7.601032 -1.755581 -0.854871" range="0.7" height="1" /> 
					<point pos="-6.134241 -1.736838 -1.913590" range="1" height="2" /> 
					<point pos="-5.533698 -1.801026 -1.201971" range="1.5" height="2" /> 
					<point pos="-5.086518 -1.746938 -1.986828" range="1" height="2" /> 
					<point pos="-4.126190 -1.694655 -2.120756" range="1.5" height="2" /> 
					<point pos="-3.625636 -1.771201 -1.275335" range="2" height="2" /> 
				</container>
				<container name="lootWeapons" lootmax="2">
					<category name="weapons" />
					<point pos="-5.230893 -1.447002 -0.552535" range="0.1" height="0.2" /> 
					<point pos="-6.382368 -1.783770 -1.002696" range="0.7" height="1" /> 
					<point pos="-6.858212 -1.741839 -1.450104" range="1" height="1" />
					<point pos="-2.930845 -1.680517 -2.063365" range="2" height="2" />
					<point pos="-4.609527 -1.812918 -1.295148" range="1.5" height="2" /> 
					<point pos="-3.567614 -1.522260 -2.499196" range="0.1" height="0.2" /> 
				</container>
			</group>
  		<group name="StaticObj_ammoboxes_single" lootmax="2">
  			<usage name="Military" />
  			<container name="lootWeapons" lootmax="2">
  						<category name="weapons" />
  						<point pos="0.012415 -0.107530 -0.091038" range="0.4" height="0.5" /> 
  						<point pos="-0.254196 -0.107530 0.627266" range="0.1" height="0.2" /> 
  						<point pos="-0.020935 -0.107530 -0.730989" range="0.1" height="0.2" /> 
  			</container>
  		</group>
  		<group name="StaticObj_ammoboxes_stacked" lootmax="1">
  			<usage name="Military" />
  			<container name="lootWeapons" lootmax="1">
  						<category name="weapons" />
  						<point pos="-0.034654 0.776729 -0.013322" range="1" height="1" /> 
  			</container>
  		</group>
  		<group name="StaticObj_Wreck_Ship_Big_FrontA" lootmax="6">
  				<usage name="Industrial" />
  				<usage name="Coast" />
  				<container name="lootFloor1" lootmax="4">
  						<category name="tools" />
  						<category name="containers" />
  						<category name="clothes" />
  						<tag name="floor" />
  						<tag name="shelves" />
  						<point pos="-6.419189 -17.062881 -2.890381" range="1.199951" height="2.000000" />
  						<point pos="-6.983640 -10.462875 -12.019044" range="1.199951" height="2.000000" />
  						<point pos="-3.400878 -10.462875 -15.116943" range="1.199951" height="2.000000" />
  						<point pos="-8.412109 -10.462875 -7.199221" range="1.199951" height="2.000000" />
  						<point pos="-3.506102 -10.462875 -10.031738" range="1.199951" height="2.000000" />
  						<point pos="1.779053 -10.462875 -7.411622" range="1.199951" height="2.000000" />
  						<point pos="-5.447021 -10.462875 -17.988037" range="1.199951" height="2.000000" />
  						<point pos="0.181642 -10.462875 -12.100099" range="1.199951" height="2.000000" />
  						<point pos="-9.760255 -8.969162 -2.999267" range="1.199951" height="2.000000" />
  						<point pos="-10.488282 -8.969162 2.778072" range="1.199951" height="2.000000" />
  						<point pos="3.168945 -8.958107 -2.925781" range="1.199951" height="2.000000" />
  				</container>
  				<container name="lootFloor2" lootmax="4">
  						<category name="tools" />
  						<category name="containers" />
  						<category name="clothes" />
  						<tag name="floor" />
  						<tag name="shelves" />
  						<point pos="3.550048 -5.662880 -6.760253" range="1.199951" height="2.000000" />
  						<point pos="-11.638917 -5.671654 3.239256" range="1.199951" height="2.000000" />
  						<point pos="-9.571289 -5.671654 0.082517" range="1.199951" height="2.000000" />
  						<point pos="5.281738 -5.671654 2.933348" range="1.199951" height="2.000000" />
  						<point pos="-9.547118 -5.662872 -9.172853" range="1.199951" height="2.000000" />
  						<point pos="-7.164063 -5.662872 -5.924560" range="0.505615" height="1.264038" />
  						<point pos="-9.547116 -5.662872 -13.672119" range="1.199951" height="2.000000" />
  						<point pos="3.280759 -5.662880 -11.974854" range="1.199951" height="2.000000" />
  						<point pos="2.837889 -5.662880 -16.870117" range="1.028125" height="2.000000" />
  						<point pos="-10.924077 -3.033089 -14.588133" range="1.199951" height="2.000000" />
  						<point pos="3.642578 -3.270432 -4.772461" range="1.199951" height="2.000000" />
  						<point pos="2.108885 -3.139740 -10.196777" range="1.199951" height="2.000000" />
  						<point pos="-10.151124 -3.274918 -4.584472" range="1.199951" height="2.000000" />
  				</container>
  				<container name="lootFloor3" lootmax="4">
  						<category name="tools" />
  						<category name="containers" />
  						<category name="clothes" />
  						<tag name="floor" />
  						<tag name="shelves" />
  						<point pos="2.860595 -2.197670 -25.912596" range="0.100000" height="0.250000" />
  						<point pos="-7.767576 -2.128906 -30.850100" range="0.100000" height="0.250000" />
  						<point pos="-9.227296 -2.249985 -25.915039" range="0.134375" height="0.335938" />
  						<point pos="-7.541012 -2.120819 -31.338619" range="0.134375" height="0.335938" />
  						<point pos="-9.391602 -2.251266 -25.410400" range="0.134375" height="0.335938" />
  						<point pos="1.213135 -2.082458 -31.385500" range="0.134375" height="0.335938" />
  						<point pos="1.397701 -2.080994 -30.874758" range="0.134375" height="0.335938" />
  						<point pos="3.066163 -2.196503 -25.446043" range="0.134375" height="0.335938" />
  						<point pos="-3.123783 -2.910545 -20.494629" range="0.932129" height="1.999996" />
  						<point pos="2.579099 -2.946297 -18.223633" range="1.199951" height="2.000000" />
  						<point pos="1.364994 -2.794647 -24.196043" range="1.199951" height="2.000000" />
  						<point pos="1.626954 -2.717445 -27.794680" range="1.199951" height="2.000000" />
  						<point pos="-0.282470 -2.603836 -32.698238" range="1.199951" height="2.000000" />
  						<point pos="-5.425293 -2.606750 -32.570072" range="1.199951" height="2.000000" />
  				</container>
  				<container name="lootfirearms" lootmax="3">
  						<category name="weapons" />
  						<category name="explosives" />
  						<point pos="4.378663 -8.948456 3.482177" range="1.199951" height="2.000000" />
  						<point pos="-1.204590 -10.462875 -18.098875" range="1.199951" height="2.000000" />
  						<point pos="-3.120360 -5.662872 -22.259035" range="1.199951" height="2.000008" />
  						<point pos="1.226563 -17.055489 3.325195" range="1.199951" height="2.000000" />
  						<point pos="-3.029541 -17.075409 0.304444" range="1.199951" height="2.000000" />
  						<point pos="5.093259 -3.046303 -14.039063" range="1.199951" height="2.000000" />
  						<point pos="-7.846675 -2.714684 -27.914309" range="1.199951" height="2.000000" />
  						<point pos="-8.402833 -2.961372 -17.615234" range="1.199951" height="2.000000" />
  						<point pos="0.607422 -3.242210 -5.954834" range="0.869873" height="2.000000" />
  						<point pos="-8.636228 -3.177734 -8.625491" range="1.199951" height="2.000000" />
  						<point pos="3.658447 -5.671654 0.041992" range="1.199951" height="2.000000" />
  						<point pos="-1.936279 -5.662872 -5.897949" range="0.479004" height="1.197510" />
  						<point pos="-6.910886 -5.662880 -24.297363" range="1.199951" height="2.000000" />
  						<point pos="0.120115 -5.662872 -24.338379" range="1.199951" height="2.000000" />
  						<point pos="-7.422365 -17.062881 2.751952" range="1.199951" height="2.000000" />
  				</container>
  		</group>
  		<group name="StaticObj_Wreck_Ship_Big_FrontB" lootmax="6">
  				<usage name="Industrial" />
  				<usage name="Coast" />
  				<container name="lootFloor1" lootmax="2">
  						<category name="tools" />
  						<category name="containers" />
  						<category name="clothes" />
  						<tag name="floor" />
  						<tag name="shelves" />
  						<point pos="-3.871092 -15.554062 -2.926759" range="1.199951" height="1.875999" />
  						<point pos="-7.565917 -15.554062 -3.071045" range="1.199951" height="1.807358" />
  						<point pos="-7.961425 -15.554062 0.554199" range="1.199951" height="1.812126" />
  						<point pos="-5.352295 -15.554062 -0.557618" range="1.199951" height="1.862556" />
  						<point pos="-2.624756 -15.554062 0.393310" range="1.199951" height="1.922905" />
  						<point pos="-4.832035 -15.550316 14.462400" range="1.199951" height="1.908638" />
  				</container>
  				<container name="lootFloor2" lootmax="2">
  						<category name="tools" />
  						<category name="containers" />
  						<category name="clothes" />
  						<tag name="floor" />
  						<tag name="shelves" />
  						<point pos="-9.916749 -7.468216 13.619381" range="0.959375" height="1.857941" />
  						<point pos="-9.938965 -7.464897 2.408446" range="0.959375" height="1.800568" />
  						<point pos="6.938963 -7.464897 -11.223877" range="1.199951" height="2.020721" />
  						<point pos="3.996337 -7.464897 -7.190917" range="1.199951" height="2.011353" />
  						<point pos="-5.445311 -7.464897 -7.485597" range="1.199951" height="1.858780" />
  						<point pos="-8.495608 -7.464897 -12.972168" range="1.199951" height="1.775391" />
  						<point pos="-8.613279 -7.464897 -7.750001" range="1.199951" height="1.791718" />
  				</container>
  				<container name="lootFloor3" lootmax="2">
  						<category name="tools" />
  						<category name="containers" />
  						<category name="clothes" />
  						<tag name="floor" />
  						<tag name="shelves" />
  						<point pos="8.503417 -4.167389 14.244140" range="1.064209" height="2.045570" />
  						<point pos="8.506104 -4.167389 7.217772" range="1.066162" height="2.040527" />
  						<point pos="-10.238037 -4.167358 2.270994" range="1.094238" height="1.793739" />
  						<point pos="-10.260499 -4.193161 12.938962" range="1.117676" height="1.960632" />
  						<point pos="-10.268798 -4.167358 5.481201" range="1.124756" height="1.804649" />
  						<point pos="-10.277099 -4.167358 9.163330" range="1.133545" height="1.817696" />
  						<point pos="8.577393 -4.167389 10.566650" range="1.137939" height="2.043236" />
  						<point pos="-7.198977 -4.167374 -13.485108" range="1.145996" height="1.800644" />
  						<point pos="8.613524 -4.167389 1.034178" range="1.174072" height="2.036530" />
  						<point pos="5.524169 -4.167389 -13.681396" range="1.179688" height="2.013077" />
  				</container>
  				<container name="lootFloor4" lootmax="1">
  						<category name="tools" />
  						<category name="containers" />
  						<category name="clothes" />
  						<tag name="floor" />
  						<tag name="shelves" />
  						<point pos="-6.745117 -1.146820 -6.634278" range="0.707273" height="1.620110" />
  						<point pos="9.108153 -1.146820 -6.806886" range="0.787500" height="1.968750" />
  						<point pos="5.041993 -1.146820 -3.192139" range="0.821875" height="1.998650" />
  						<point pos="9.000244 -1.146820 -3.247072" range="0.890625" height="2.031113" />
  						<point pos="8.575927 -1.146820 -5.078125" range="0.984440" height="2.028023" />
  				</container>
  				<container name="lootfirearms" lootmax="3">
  						<category name="explosives" />
  						<category name="weapons" />
  						<point pos="-7.870358 -15.554062 14.052245" range="1.199951" height="1.862556" />
  						<point pos="-6.483398 -7.464897 -3.036133" range="1.199951" height="1.853096" />
  						<point pos="-2.397949 -1.146820 -3.645996" range="1.199951" height="1.916344" />
  						<point pos="-2.060547 -1.146820 -6.357422" range="1.199951" height="1.913635" />
  						<point pos="-9.622558 -4.167351 -13.529054" range="1.199951" height="1.749832" />
  						<point pos="7.918213 -4.167389 -9.878419" range="1.199951" height="2.025803" />
  						<point pos="1.011230 -1.146820 -4.791992" range="1.199951" height="1.983330" />
  						<point pos="-5.969973 -15.554062 11.485106" range="1.199951" height="1.892960" />
  						<point pos="-10.208496 -1.146820 -3.540042" range="1.199951" height="1.753876" />
  						<point pos="-7.328366 -4.167374 -10.221926" range="1.199951" height="1.809685" />
  						<point pos="6.195312 -7.464890 -3.034180" range="1.199951" height="2.023506" />
  						<point pos="1.020019 -15.554062 8.783936" range="1.199951" height="1.583023" />
  						<point pos="8.479738 -7.464897 15.260987" range="1.076542" height="2.000000" />
  				</container>
  		</group>
  		<group name="StaticObj_Wreck_Ship_Big_BackA" lootmax="6">
  				<usage name="Industrial" />
  				<usage name="Coast" />
  				<container name="lootFloor1" lootmax="2">
  						<category name="tools" />
  						<category name="containers" />
  						<category name="clothes" />
  						<tag name="floor" />
  						<tag name="shelves" />
  						<point pos="-1.311035 -17.003929 -1.717529" range="1.199951" height="2.000023" />
  						<point pos="-6.891846 -17.003929 -1.521974" range="1.199951" height="2.000023" />
  						<point pos="-4.176759 -17.003929 -3.900880" range="1.199951" height="2.000023" />
  						<point pos="-1.294191 -17.003929 -10.496095" range="1.199951" height="2.000023" />
  						<point pos="-7.496825 -17.003929 -12.462158" range="1.199951" height="2.000023" />
  				</container>
  				<container name="lootFloor2" lootmax="2">
  						<category name="tools" />
  						<category name="containers" />
  						<category name="clothes" />
  						<tag name="floor" />
  						<tag name="shelves" />
  						<point pos="-5.612305 -8.910210 0.563720" range="1.199951" height="2.000008" />
  						<point pos="-2.671631 -8.910217 -17.678955" range="0.340625" height="0.851563" />
  						<point pos="-8.769529 -8.910210 -4.629397" range="0.959375" height="2.000008" />
  						<point pos="-2.705323 -8.910210 -14.357667" range="1.062500" height="2.000008" />
  						<point pos="1.808349 -8.910210 -14.361816" range="1.062500" height="2.000008" />
  						<point pos="9.562255 -8.910210 -5.815673" range="1.131250" height="2.000008" />
  				</container>
  				<container name="lootFloor3" lootmax="2">
  						<category name="tools" />
  						<category name="containers" />
  						<category name="clothes" />
  						<tag name="floor" />
  						<tag name="shelves" />
  						<point pos="9.590332 -5.612701 -2.988526" range="0.991455" height="2.000000" />
  						<point pos="-9.107422 -5.612701 -6.806885" range="0.787500" height="1.968750" />
  						<point pos="-9.031251 -5.612701 1.214111" range="1.028125" height="2.000000" />
  						<point pos="9.753417 -5.612701 -14.306396" range="1.134521" height="2.000000" />
  						<point pos="9.799560 -5.612701 -7.915528" range="1.199951" height="2.000000" />
  						<point pos="-9.214358 -5.612701 -12.270264" range="1.199951" height="2.000000" />
  						<point pos="-9.230713 -5.612701 -4.340820" range="1.199951" height="2.000000" />
  						<point pos="9.795410 -5.612701 1.856199" range="1.199951" height="2.000000" />
  				</container>
  				<container name="lootfirearms" lootmax="3">
  						<category name="explosives" />
  						<category name="weapons" />
  						<point pos="-2.041016 -17.003929 -6.854737" range="1.199951" height="2.000023" />
  						<point pos="-7.072265 -17.003929 -8.246338" range="1.199951" height="2.000023" />
  						<point pos="-5.496581 -2.596138 -15.438477" range="1.199951" height="2.000008" />
  						<point pos="0.458985 -2.596138 -16.962891" range="1.199951" height="2.000008" />
  						<point pos="6.937987 -2.596138 -16.020508" range="1.199951" height="2.000008" />
  						<point pos="-3.401855 -5.612701 1.038330" range="1.199951" height="2.000000" />
  						<point pos="2.824463 -5.612701 0.812988" range="1.199951" height="2.000000" />
  						<point pos="-6.273195 -8.911217 -17.441404" range="0.821875" height="2.000000" />
  				</container>
  		</group>
  		<group name="StaticObj_Wreck_Ship_Big_BackB" lootmax="6">
  				<usage name="Industrial" />
  				<usage name="Coast" />
  				<container name="lootFloor1" lootmax="2">
  						<category name="tools" />
  						<category name="containers" />
  						<category name="clothes" />
  						<tag name="floor" />
  						<tag name="shelves" />
  						<point pos="-4.670908 -7.888664 26.930416" range="1.199951" height="2.000000" />
  						<point pos="1.020757 -7.888657 20.576660" range="1.199951" height="2.000000" />
  						<point pos="-6.341553 -7.888657 15.273925" range="1.199951" height="2.000000" />
  						<point pos="4.479253 -7.888664 26.186523" range="1.199951" height="2.000000" />
  				</container>
  				<container name="lootFloor2" lootmax="2">
  						<category name="tools" />
  						<category name="containers" />
  						<category name="clothes" />
  						<tag name="floor" />
  						<tag name="shelves" />
  						<point pos="6.305418 -4.088692 27.368408" range="1.199951" height="2.000000" />
  						<point pos="-8.123780 -4.088669 13.812499" range="1.199951" height="2.000000" />
  						<point pos="-6.876952 -4.088661 19.833986" range="1.199951" height="2.000000" />
  						<point pos="2.284424 -4.088654 13.596435" range="1.199951" height="2.000000" />
  						<point pos="7.741943 -4.088669 15.014649" range="1.199951" height="2.000000" />
  				</container>
  				<container name="lootFloor3" lootmax="4">
  						<category name="tools" />
  						<category name="containers" />
  						<category name="clothes" />
  						<tag name="floor" />
  						<tag name="shelves" />
  						<point pos="-5.288336 -1.387939 28.207520" range="0.546875" height="1.367188" />
  						<point pos="-0.081791 -1.387939 28.079592" range="0.650000" height="1.625000" />
  						<point pos="2.351326 -1.387939 28.066404" range="0.684375" height="1.710938" />
  						<point pos="-2.953362 -1.387939 28.055174" range="0.716064" height="1.790160" />
  						<point pos="9.094975 -1.387939 16.827879" range="0.959375" height="2.000000" />
  						<point pos="8.014406 -1.387939 23.336426" range="1.199951" height="2.000000" />
  						<point pos="-7.339844 -1.387939 25.094725" range="1.199951" height="2.000000" />
  						<point pos="-7.368405 -1.387939 21.431643" range="1.199951" height="2.000000" />
  						<point pos="-7.030031 -1.387939 17.625488" range="1.199951" height="2.000000" />
  						<point pos="7.829099 -1.387939 26.640383" range="1.199951" height="2.000000" />
  						<point pos="6.193851 -1.387939 18.488279" range="1.199951" height="2.000000" />
  						<point pos="8.316410 -0.799210 18.575926" range="0.100000" height="0.250000" />
  						<point pos="-8.709226 -0.792671 18.036379" range="0.134375" height="0.335938" />
  						<point pos="-0.145512 1.107010 12.318849" range="0.937055" height="2.000000" />
  				</container>
  				<container name="lootfirearms" lootmax="2">
  						<category name="explosives" />
  						<category name="weapons" />
  						<point pos="5.640379 -7.888657 17.344482" range="1.199951" height="2.000000" />
  						<point pos="-8.754393 -0.798393 18.545168" range="0.134375" height="0.335938" />
  						<point pos="4.331551 -1.387939 28.181149" range="0.546875" height="1.367188" />
  						<point pos="-6.713624 -4.088661 26.956787" range="1.199951" height="2.000000" />
  				</container>
  		</group>
  		<group name="StaticObj_Wreck_Ship_Big_Castle" lootmax="25">
  				<usage name="Industrial" />
  				<usage name="Coast" />
  				<container name="lootFloor1" lootmax="2">
  						<category name="tools" />
  						<category name="containers" />
  						<category name="clothes" />
  						<tag name="floor" />
  						<point pos="-3.113038 -16.946526 2.968260" range="1.199951" height="2.000343" />
  						<point pos="3.030518 -16.946526 3.119628" range="1.199951" height="2.000343" />
  						<point pos="-1.461914 -14.254990 -0.258301" range="1.199951" height="2.000000" />
  						<point pos="-3.541015 -14.254990 -3.188477" range="1.199951" height="2.000000" />
  				</container>
  				<container name="lootFloor2" lootmax="5">
  						<category name="tools" />
  						<category name="containers" />
  						<category name="clothes" />
  						<tag name="floor" />
  						<point pos="-0.229492 -11.545486 -2.848633" range="1.199951" height="2.000000" />
  						<point pos="-3.829101 -11.545486 -2.819092" range="1.199951" height="2.000000" />
  						<point pos="-7.532472 -11.545486 -2.286865" range="1.199951" height="2.000000" />
  						<point pos="7.163086 -11.545486 13.320312" range="1.199951" height="2.000015" />
  						<point pos="6.944580 -11.545486 5.753660" range="1.199951" height="2.000015" />
  						<point pos="-6.811279 -11.545486 -6.317383" range="1.199951" height="2.000000" />
  						<point pos="5.055665 -11.545486 -6.264648" range="1.199951" height="2.000008" />
  						<point pos="-7.715328 -11.545486 14.718505" range="1.115234" height="2.000000" />
  						<point pos="-7.738038 -11.545486 10.862791" range="1.137939" height="2.000000" />
  						<point pos="4.048583 -11.545486 -2.850097" range="1.151367" height="2.000000" />
  						<point pos="-6.194337 -11.545486 6.358641" range="1.094238" height="2.000000" />
  						<point pos="-5.771727 -11.545486 11.412842" range="0.671143" height="1.677858" />
  						<point pos="-5.800540 -11.545486 14.311766" range="0.699463" height="1.748657" />
  						<point pos="-9.809329 -11.545479 14.487790" range="0.809570" height="2.000008" />
  						<point pos="9.914554 -11.545486 12.905761" range="0.821875" height="2.000015" />
  						<point pos="-9.867434 -11.545486 5.994139" range="0.867676" height="2.000015" />
  						<point pos="9.885742 -11.545486 3.026122" range="0.885742" height="2.000015" />
  						<point pos="8.010986 -11.545486 -2.520996" range="0.901367" height="1.997169" />
  						<point pos="3.174809 -11.545486 19.069578" range="0.996094" height="1.999847" />
  						<point pos="-7.343506 -11.545486 18.895750" range="1.185303" height="2.000015" />
  						<point pos="-7.676270 -11.545486 2.200927" range="1.199951" height="2.000000" />
  				</container>
  				<container name="lootFloor3" lootmax="2">
  						<category name="tools" />
  						<category name="containers" />
  						<category name="clothes" />
  						<tag name="floor" />
  						<point pos="-9.657959 -8.846199 0.290283" range="1.152588" height="2.000008" />
  						<point pos="9.722417 -8.846199 14.657957" range="1.028125" height="1.902893" />
  						<point pos="9.679443 -8.846199 16.924801" range="1.062500" height="1.966789" />
  						<point pos="-9.487304 -8.846199 16.964355" range="0.909378" height="2.000008" />
  						<point pos="-3.586914 -8.846199 -2.727295" range="0.986816" height="2.000008" />
  						<point pos="9.808106 -8.846199 2.570312" range="0.988770" height="2.000008" />
  						<point pos="9.202638 -8.846199 7.356934" range="0.702082" height="1.755205" />
  						<point pos="-2.588379 -8.846199 2.118896" range="1.199951" height="2.000008" />
  						<point pos="2.500976 -8.846199 1.609130" range="1.199951" height="2.000008" />
  						<point pos="5.703856 -8.846199 -2.347656" range="1.195557" height="2.000008" />
  						<point pos="-9.367188 -8.846199 3.233644" range="1.199951" height="2.000008" />
  						<point pos="-1.165283 -8.846199 -2.626709" range="1.199951" height="2.000008" />
  						<point pos="-5.991456 -8.846199 18.779539" range="1.199951" height="2.000008" />
  						<point pos="6.071536 -8.846199 18.879883" range="1.199951" height="2.000008" />
  						<point pos="-9.530272 -8.846199 14.855711" range="1.199951" height="2.000008" />
  						<point pos="9.501221 -8.846199 0.260254" range="1.199951" height="2.000008" />
  						<point pos="3.433351 -8.846199 4.615966" range="1.199951" height="2.000008" />
  						<point pos="-3.488769 -8.846199 4.794921" range="1.199951" height="1.709892" />
  						<point pos="-7.747803 -7.863258 18.816162" range="0.203125" height="0.507813" />
  						<point pos="-7.743895 -7.863258 13.188231" range="0.203125" height="0.507813" />
  						<point pos="7.769779 -7.863266 12.589844" range="0.203125" height="0.507813" />
  						<point pos="7.739991 -7.863266 18.218994" range="0.203125" height="0.507813" />
  						<point pos="9.790774 -6.214699 16.876951" range="1.096875" height="2.631523" />
  						<point pos="-3.563233 -6.145805 1.072508" range="1.199951" height="1.516701" />
  						<point pos="2.759278 -6.145805 1.055175" range="1.199951" height="2.000008" />
  						<point pos="9.486084 -6.145805 3.893065" range="1.199951" height="2.000015" />
  						<point pos="7.551514 -6.145805 5.782958" range="1.199951" height="2.000015" />
  						<point pos="9.397218 -6.145805 1.127440" range="1.199951" height="2.000015" />
  						<point pos="7.427978 -6.145805 -1.892823" range="1.199951" height="2.000008" />
  						<point pos="-1.783447 -6.145805 -1.558594" range="1.199951" height="2.000008" />
  						<point pos="0.985840 -6.145805 -2.501221" range="1.199951" height="2.000008" />
  						<point pos="-8.404299 -6.145805 5.824703" range="1.199951" height="2.000015" />
  						<point pos="3.587893 -6.145805 12.878173" range="1.199951" height="2.000008" />
  						<point pos="-3.371095 -6.145805 12.861815" range="1.199951" height="2.000008" />
  						<point pos="9.745367 -5.753654 14.217037" range="1.199951" height="2.193985" />
  						<point pos="-9.861814 -5.753647 14.197510" range="1.199951" height="2.197990" />
  						<point pos="-9.762943 -5.753647 17.273436" range="1.199951" height="2.200157" />
  				</container>
  				<container name="lootFloor4" lootmax="3">
  						<category name="tools" />
  						<category name="containers" />
  						<category name="clothes" />
  						<tag name="floor" />
  						<point pos="6.671875 -3.446808 -1.537110" range="1.185059" height="2.000015" />
  						<point pos="1.327392 -3.446800 -2.420410" range="1.199951" height="2.000008" />
  						<point pos="-1.576904 -3.446800 -2.104492" range="1.199951" height="2.000008" />
  						<point pos="-7.189697 -3.446800 5.868161" range="1.199951" height="2.000008" />
  						<point pos="6.981446 -3.446800 5.491210" range="1.199951" height="2.000008" />
  						<point pos="0.002441 -0.753403 -2.931152" range="1.176270" height="2.000000" />
  						<point pos="-4.850342 -0.752792 1.496338" range="1.199951" height="1.996948" />
  						<point pos="6.691651 -0.752769 1.914794" range="1.199951" height="1.996803" />
  				</container>
  				<container name="lootshelves1" lootmax="4">
  						<category name="tools" />
  						<category name="containers" />
  						<category name="clothes" />
  						<category name="food" />
  						<category name="books" />
  						<tag name="shelves" />
  						<point pos="-2.575195 -2.340828 -3.474853" range="0.100000" height="0.250000" />
  						<point pos="0.304931 -2.112373 -3.423340" range="0.100000" height="0.250000" />
  						<point pos="-0.296631 -2.124092 -3.399658" range="0.100000" height="0.250000" />
  						<point pos="4.712402 -2.325745 -3.194092" range="0.134375" height="0.335938" />
  						<point pos="5.734863 -2.342789 -2.998780" range="0.134375" height="0.335938" />
  						<point pos="7.764403 -13.396255 -3.340088" range="0.134375" height="0.264999" />
  						<point pos="-4.462891 -2.412804 -2.990724" range="0.134375" height="0.335938" />
  						<point pos="3.175781 -2.363510 -3.294677" range="0.134375" height="0.335938" />
  						<point pos="4.048584 -2.357674 -3.189942" range="0.134375" height="0.335938" />
  				</container>
  				<container name="lootshelves2" lootmax="10">
  						<category name="tools" />
  						<category name="containers" />
  						<category name="clothes" />
  						<category name="food" />
  						<category name="books" />
  						<tag name="shelves" />
  						<point pos="7.313476 -12.659645 -0.100098" range="0.151367" height="0.164352" />
  						<point pos="7.748290 -13.855202 3.720214" range="0.237500" height="0.593750" />
  						<point pos="-8.710694 -13.021004 10.451413" range="0.271875" height="0.679688" />
  						<point pos="8.809082 -13.810997 1.255615" range="0.306250" height="0.533005" />
  						<point pos="8.959718 -13.810997 4.935058" range="0.306250" height="0.533066" />
  						<point pos="-8.962891 -13.020676 8.585445" range="0.306250" height="0.765625" />
  						<point pos="8.910645 -13.020340 17.207518" range="0.306250" height="0.765625" />
  						<point pos="8.003905 -13.021248 -2.248779" range="0.340625" height="0.834351" />
  						<point pos="8.328368 -13.021095 1.201660" range="0.340625" height="0.834198" />
  						<point pos="8.058106 -13.021278 -0.458497" range="0.340625" height="0.851563" />
  						<point pos="-8.173342 -13.021286 20.403807" range="0.340625" height="0.851563" />
  						<point pos="-9.058840 -13.810997 17.214109" range="0.340625" height="0.533066" />
  						<point pos="-8.477044 -13.021156 17.196779" range="0.340625" height="0.851563" />
  						<point pos="-9.594240 -13.810997 8.533690" range="0.340625" height="0.533607" />
  						<point pos="9.580077 -13.019890 7.010254" range="0.340625" height="0.851563" />
  						<point pos="8.629150 -13.810997 7.007324" range="0.340625" height="0.532486" />
  						<point pos="-8.777833 -13.810997 10.523191" range="0.340625" height="0.532600" />
  						<point pos="-8.799561 -13.021225 1.283202" range="0.340625" height="0.851563" />
  						<point pos="-8.437499 -13.021194 15.527830" range="0.443750" height="0.834328" />
  						<point pos="8.272708 -13.810997 17.280272" range="0.375000" height="0.532410" />
  						<point pos="9.009766 -13.810997 2.471191" range="0.375000" height="0.532364" />
  						<point pos="8.283446 -13.021271 4.889405" range="0.375000" height="0.834366" />
  						<point pos="-8.599121 -13.810997 8.508545" range="0.375000" height="0.532402" />
  						<point pos="9.157470 -13.810997 -0.427003" range="0.375000" height="0.533569" />
  						<point pos="-9.296388 -13.810997 18.546631" range="0.375000" height="0.533493" />
  						<point pos="-9.669926 -13.810997 10.531491" range="0.375000" height="0.533676" />
  						<point pos="-8.241457 -13.021301 18.537594" range="0.375000" height="0.937500" />
  						<point pos="-9.172115 -13.810997 20.435791" range="0.375000" height="0.533432" />
  						<point pos="9.161864 -13.810997 -2.212159" range="0.375000" height="0.533669" />
  						<point pos="-9.202641 -13.810997 15.970212" range="0.409375" height="0.533386" />
  						<point pos="-8.686522 -13.810997 1.278563" range="0.340625" height="0.532158" />
  						<point pos="7.800780 -14.151253 -3.369386" range="0.100000" height="0.250000" />
  						<point pos="7.299072 -14.210243 -0.141847" range="0.155762" height="0.389405" />
  				</container>
  				<container name="lootweapons" lootmax="8">
  						<category name="weapons" />
  						<category name="explosives" />
  						<point pos="7.395996 -14.210243 17.488770" range="0.156738" height="0.391845" />
  						<point pos="8.127929 -13.021286 17.170654" range="0.271875" height="0.679688" />
  						<point pos="9.339598 -13.810997 17.274660" range="0.375000" height="0.533699" />
  						<point pos="10.142577 -8.846199 9.094237" range="0.663330" height="1.658325" />
  						<point pos="-9.948973 -8.846199 9.185547" range="0.756348" height="1.890870" />
  						<point pos="9.770021 -11.545486 19.123777" range="0.769531" height="1.923828" />
  						<point pos="9.807372 -11.545486 7.082032" range="0.806885" height="2.000015" />
  						<point pos="-9.922851 -11.545479 11.372313" range="0.821875" height="2.000008" />
  						<point pos="8.431152 -8.846199 3.786376" range="0.849007" height="2.000008" />
  						<point pos="10.045654 -3.446800 3.267090" range="0.856250" height="2.000008" />
  						<point pos="9.917237 -8.846199 5.934570" range="0.890137" height="2.000008" />
  						<point pos="3.559570 -8.846199 -2.686035" range="0.959473" height="2.000008" />
  						<point pos="-0.119386 -8.846199 19.149170" range="0.997314" height="2.000008" />
  						<point pos="-0.878903 -11.545486 19.077148" range="1.003418" height="1.998283" />
  						<point pos="3.921390 -6.145805 16.830324" range="1.028125" height="2.000008" />
  						<point pos="-4.178952 -3.446800 7.607911" range="1.131250" height="2.000008" />
  						<point pos="-9.639163 -6.145805 3.654293" range="1.131250" height="2.000015" />
  						<point pos="6.574951 -0.753387 -2.518800" range="1.133301" height="1.999924" />
  						<point pos="4.863037 -6.145805 -2.414063" range="1.137207" height="2.000008" />
  						<point pos="-5.715821 -8.846199 -1.993164" range="1.184082" height="2.000008" />
  						<point pos="-6.643311 -0.753387 -2.446045" range="1.196045" height="1.999924" />
  						<point pos="-4.661377 -6.145805 -1.842042" range="1.199951" height="2.000008" />
  						<point pos="-9.366700 -6.145805 -1.220948" range="1.199951" height="2.000008" />
  						<point pos="6.881595 -11.545486 9.634521" range="1.199951" height="2.000015" />
  						<point pos="4.412598 -3.446800 7.078124" range="1.199951" height="2.000008" />
  						<point pos="-9.426761 -8.846199 6.836421" range="1.199951" height="2.000008" />
  						<point pos="-8.343507 -8.846199 -1.730469" range="1.199951" height="2.000008" />
  						<point pos="-2.709473 -11.545486 -6.245606" range="1.199951" height="2.000008" />
  						<point pos="-0.119629 -16.946526 3.138427" range="1.199951" height="2.000343" />
  						<point pos="-9.508545 -3.446808 2.734617" range="1.199951" height="2.000015" />
  						<point pos="8.260986 -8.846199 -1.812501" range="1.199951" height="2.000008" />
  						<point pos="-7.561036 -6.145805 0.970702" range="1.199951" height="2.000000" />
  						<point pos="-0.079839 -6.145805 15.217529" range="1.199951" height="2.000000" />
  						<point pos="7.847900 -11.545486 2.033935" range="1.058349" height="2.000000" />
  						<point pos="8.375736 -11.545486 18.229002" range="0.456299" height="1.140747" />
  						<point pos="-3.165771 -16.946526 6.819825" range="1.038574" height="1.508690" />
  						<point pos="7.575199 -11.545486 19.307861" range="0.774170" height="1.935425" />
  						<point pos="9.220947 -13.020958 2.503172" range="0.443402" height="1.046387" />
  						<point pos="2.941162 -16.946526 6.952148" range="0.906250" height="1.600876" />
  						<point pos="-3.865231 -6.145805 16.585203" range="1.199951" height="2.000008" />
  						<point pos="1.294434 -8.846199 -2.249512" range="1.199951" height="2.000008" />
  				</container>
  		</group>
After adding those to your protto,
Add the XMCOilRig.xml code in your mapgrouppos to allow the mod to spawn loot
Tip: Use <!-- --> to organize vanilla and any other modded loot spawns, here is an example

<!-- Objects -->
    <group name="Object1" pos="0. 0.0 0.0" rpy="-0 0 67.0361" a="22.9639" />
    <group name="Onject2" pos="10.0 10.0 10.0" rpy="-0 0 84.0529" a="5.9471" />
    <group name="Object3" pos="100.0 100.0 100.0" rpy="-0 0 -91.1432" a="-178.857" />
<!-- Vanilla -->
    <group name="Land_Misc_FeedShack" pos="80.262581 113.793480 4422.178223" rpy="-0.000000 0.000000 -70.013718" a="160.013718" />
    <group name="Land_Misc_FeedShack" pos="80.261421 411.262756 10449.132813" rpy="-0.000000 0.000000 -58.923214" a="148.923203" />
    <group name="Land_Shed_W2" pos="174.522446 103.526039 2380.768066" rpy="-0.000000 0.000000 160.642838" a="-70.642845" />
    <group name="Land_Misc_FeedShack" pos="151.014359 56.180706 3655.147217" rpy="-0.000000 0.000000 -175.400726" a="-94.599258" />

Add a new entry in the gameplay file under object spawner
If you have other json files, make sure to put a comma after each entry, just not the last one
Example:

		"objectSpawnersArr": [
			"/custom/Object1.json",
			"/custom/Object2.json",
			"/custom/XMCOilRig.json"
		],

After your map file finished uploading, 
Add/upload the XMCOilRig.json file in the custom folder
make sure to validate your updated files before uploading.
And upload your updated gameplay.json, mapgrouppos.xml, and mapgroupprotto.xml (Wait for each one to finish uploading before uploading the next one)
After every file is uploaded, wait 5-10 minutes for your server (for the areaflags.map file to work) then press start on your server.

Now if you done everything correctly, you will have an oil rig that also will spawn loot

Additional Info:
Oil Rig is located at 6000 / 500
Shipwreck is located at 13000 / 3500
The areaflags.map file turns the oil rig to spawn unique tier loot and turns the oil area into military loot. So you will see military loot in construction buildings and containers.
Nothing else was changed in the map file, everything else in the file is unchanged.
You are able to get on the oil rig if you swim to it in version 1.25, it has a boating dock for boats in version 1.26
