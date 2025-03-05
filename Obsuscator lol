--[[
 .____                  ________ ___.    _____                           __                
 |    |    __ _______   \_____  \\_ |___/ ____\_ __  ______ ____ _____ _/  |_  ___________ 
 |    |   |  |  \__  \   /   |   \| __ \   __\  |  \/  ___// ___\\__  \\   __\/  _ \_  __ \
 |    |___|  |  // __ \_/    |    \ \_\ \  | |  |  /\___ \\  \___ / __ \|  | (  <_> )  | \/
 |_______ \____/(____  /\_______  /___  /__| |____//____  >\___  >____  /__|  \____/|__|   
         \/          \/         \/    \/                \/     \/     \/                   
          \_Welcome to LuaObfuscator.com   (Alpha 0.10.8) ~  Much Love, Ferib 

]]--

local v0 = string.char;
local v1 = string.byte;
local v2 = string.sub;
local v3 = bit32 or bit;
local v4 = v3.bxor;
local v5 = table.concat;
local v6 = table.insert;
local function v7(v24, v25)
	local v26 = {};
	for v41 = 1, #v24 do
		v6(v26, v0(v4(v1(v2(v24, v41, v41 + 1)), v1(v2(v25, 1 + (v41 % #v25), 1 + (v41 % #v25) + 1))) % 256));
	end
	return v5(v26);
end
local v8 = tonumber;
local v9 = string.byte;
local v10 = string.char;
local v11 = string.sub;
local v12 = string.gsub;
local v13 = string.rep;
local v14 = table.concat;
local v15 = table.insert;
local v16 = math.ldexp;
local v17 = getfenv or function()
	return _ENV;
end;
local v18 = setmetatable;
local v19 = pcall;
local v20 = select;
local v21 = unpack or table.unpack;
local v22 = tonumber;
local function v23(v27, v28, ...)
	local v29 = 1;
	local v30;
	v27 = v12(v11(v27, 5), v7("\178\177", "\179\156\159\17\52\214"), function(v42)
		if (v9(v42, 2) == 81) then
			local v101 = 0;
			while true do
				if (0 == v101) then
					v30 = v8(v11(v42, 1, 2 - 1));
					return "";
				end
			end
		else
			local v102 = 0;
			local v103;
			while true do
				if (v102 == 0) then
					v103 = v10(v8(v42, 16));
					if v30 then
						local v125 = 0;
						local v126;
						while true do
							if (v125 == 1) then
								return v126;
							end
							if (v125 == 0) then
								v126 = v13(v103, v30);
								v30 = nil;
								v125 = 1;
							end
						end
					else
						return v103;
					end
					break;
				end
			end
		end
	end);
	local function v31(v43, v44, v45)
		if v45 then
			local v104 = 0;
			local v105;
			while true do
				if (v104 == 0) then
					v105 = (v43 / (2 ^ (v44 - 1))) % (2 ^ (((v45 - 1) - (v44 - 1)) + 1));
					return v105 - (v105 % 1);
				end
			end
		else
			local v106 = 0;
			local v107;
			while true do
				if (0 == v106) then
					v107 = 2 ^ (v44 - 1);
					return (((v43 % (v107 + v107)) >= v107) and 1) or 0;
				end
			end
		end
	end
	local function v32()
		local v46 = 0;
		local v47;
		while true do
			if (v46 == 0) then
				v47 = v9(v27, v29, v29);
				v29 = v29 + 1;
				v46 = 1;
			end
			if (v46 == 1) then
				return v47;
			end
		end
	end
	local function v33()
		local v48 = 0;
		local v49;
		local v50;
		while true do
			if (v48 == 0) then
				v49, v50 = v9(v27, v29, v29 + 2);
				v29 = v29 + 2;
				v48 = 1;
			end
			if (v48 == 1) then
				return (v50 * 256) + v49;
			end
		end
	end
	local function v34()
		local v51, v52, v53, v54 = v9(v27, v29, v29 + 3);
		v29 = v29 + 4;
		return (v54 * (48013535 - 31236319)) + (v53 * 65536) + (v52 * 256) + v51;
	end
	local function v35()
		local v55 = 0;
		local v56;
		local v57;
		local v58;
		local v59;
		local v60;
		local v61;
		while true do
			if (v55 == 1) then
				v58 = 1;
				v59 = (v31(v57, 1, 20) * (2 ^ 32)) + v56;
				v55 = 2;
			end
			if (v55 == 2) then
				v60 = v31(v57, 21, 59 - 28);
				v61 = ((v31(v57, 32) == (2 - 1)) and -1) or 1;
				v55 = 3;
			end
			if (v55 == 3) then
				if (v60 == 0) then
					if (v59 == 0) then
						return v61 * 0;
					else
						v60 = 1;
						v58 = 0;
					end
				elseif (v60 == 2047) then
					return ((v59 == 0) and (v61 * (1 / 0))) or (v61 * NaN);
				end
				return v16(v61, v60 - (1642 - (555 + 64))) * (v58 + (v59 / (2 ^ 52)));
			end
			if (v55 == 0) then
				v56 = v34();
				v57 = v34();
				v55 = 1;
			end
		end
	end
	local function v36(v62)
		local v63 = 0;
		local v64;
		local v65;
		while true do
			if (v63 == 1) then
				v64 = v11(v27, v29, (v29 + v62) - 1);
				v29 = v29 + v62;
				v63 = 2;
			end
			if (v63 == 3) then
				return v14(v65);
			end
			if (v63 == 0) then
				v64 = nil;
				if not v62 then
					local v121 = 0;
					while true do
						if (v121 == 0) then
							v62 = v34();
							if (v62 == 0) then
								return "";
							end
							break;
						end
					end
				end
				v63 = 1;
			end
			if (v63 == 2) then
				v65 = {};
				for v114 = 1, #v64 do
					v65[v114] = v10(v9(v11(v64, v114, v114)));
				end
				v63 = 3;
			end
		end
	end
	local v37 = v34;
	local function v38(...)
		return {...}, v20("#", ...);
	end
	local function v39()
		local v66 = {};
		local v67 = {};
		local v68 = {};
		local v69 = {v66,v67,nil,v68};
		local v70 = v34();
		local v71 = {};
		for v79 = 1, v70 do
			local v80 = 0;
			local v81;
			local v82;
			while true do
				if (1 == v80) then
					if (v81 == 1) then
						v82 = v32() ~= 0;
					elseif (v81 == 2) then
						v82 = v35();
					elseif (v81 == 3) then
						v82 = v36();
					end
					v71[v79] = v82;
					break;
				end
				if (v80 == 0) then
					v81 = v32();
					v82 = nil;
					v80 = 1;
				end
			end
		end
		v69[3] = v32();
		for v83 = 1, v34() do
			local v84 = v32();
			if (v31(v84, 1, 1) == 0) then
				local v110 = 0;
				local v111;
				local v112;
				local v113;
				while true do
					if (v110 == 0) then
						v111 = v31(v84, 570 - (367 + 201), 930 - (214 + 713));
						v112 = v31(v84, 4, 2 + 4);
						v110 = 1;
					end
					if (2 == v110) then
						if (v31(v112, 1, 1) == 1) then
							v113[1639 - (1523 + 114)] = v71[v113[2]];
						end
						if (v31(v112, 2, 2) == (1 + 0)) then
							v113[3] = v71[v113[3]];
						end
						v110 = 3;
					end
					if (v110 == 1) then
						v113 = {v33(),v33(),nil,nil};
						if (v111 == 0) then
							local v131 = 0;
							while true do
								if (v131 == 0) then
									v113[3] = v33();
									v113[4] = v33();
									break;
								end
							end
						elseif (v111 == 1) then
							v113[3] = v34();
						elseif (v111 == (879 - (282 + 595))) then
							v113[3] = v34() - (2 ^ 16);
						elseif (v111 == 3) then
							local v138 = 0;
							while true do
								if (v138 == 0) then
									v113[3] = v34() - (2 ^ 16);
									v113[4] = v33();
									break;
								end
							end
						end
						v110 = 2;
					end
					if (v110 == 3) then
						if (v31(v112, 3, 3 - 0) == 1) then
							v113[4] = v71[v113[4]];
						end
						v66[v83] = v113;
						break;
					end
				end
			end
		end
		for v85 = 1, v34() do
			v67[v85 - (1066 - (68 + 997))] = v39();
		end
		return v69;
	end
	local function v40(v73, v74, v75)
		local v76 = v73[1];
		local v77 = v73[2];
		local v78 = v73[1273 - (226 + 1044)];
		return function(...)
			local v87 = v76;
			local v88 = v77;
			local v89 = v78;
			local v90 = v38;
			local v91 = 1;
			local v92 = -(4 - 3);
			local v93 = {};
			local v94 = {...};
			local v95 = v20("#", ...) - (118 - (32 + 85));
			local v96 = {};
			local v97 = {};
			for v108 = 0, v95 do
				if (v108 >= v89) then
					v93[v108 - v89] = v94[v108 + 1];
				else
					v97[v108] = v94[v108 + 1];
				end
			end
			local v98 = (v95 - v89) + 1;
			local v99;
			local v100;
			while true do
				local v109 = 0;
				while true do
					if (v109 == 0) then
						v99 = v87[v91];
						v100 = v99[1];
						v109 = 1;
					end
					if (v109 == 1) then
						if (v100 <= 29) then
							if (v100 <= (14 + 0)) then
								if (v100 <= 6) then
									if (v100 <= 2) then
										if (v100 <= (0 + 0)) then
											local v139 = 0;
											local v140;
											local v141;
											local v142;
											local v143;
											while true do
												if (v139 == 1) then
													v91 = v91 + 1;
													v99 = v87[v91];
													v97[v99[2]] = v99[7 - 4];
													v91 = v91 + 1;
													v139 = 2;
												end
												if (v139 == 2) then
													v99 = v87[v91];
													v97[v99[2]] = v99[5 - 2];
													v91 = v91 + 1;
													v99 = v87[v91];
													v139 = 3;
												end
												if (4 == v139) then
													for v328 = v143, v92 do
														local v329 = 0;
														while true do
															if (v329 == 0) then
																v140 = v140 + 1;
																v97[v328] = v141[v140];
																break;
															end
														end
													end
													v91 = v91 + 1;
													v99 = v87[v91];
													v143 = v99[2];
													v139 = 5;
												end
												if (v139 == 0) then
													v140 = nil;
													v141, v142 = nil;
													v143 = nil;
													v97[v99[2]] = v74[v99[960 - (892 + 65)]];
													v139 = 1;
												end
												if (v139 == 5) then
													v97[v143](v21(v97, v143 + 1, v92));
													break;
												end
												if (v139 == 3) then
													v143 = v99[2];
													v141, v142 = v90(v97[v143](v21(v97, v143 + 1, v99[3])));
													v92 = (v142 + v143) - 1;
													v140 = 0;
													v139 = 4;
												end
											end
										elseif (v100 == (1 - 0)) then
											v97[v99[352 - (87 + 263)]][v97[v99[3]]] = v97[v99[184 - (67 + 113)]];
										else
											local v151;
											local v152;
											local v153;
											v75[v99[3]] = v97[v99[2]];
											v91 = v91 + 1;
											v99 = v87[v91];
											v97[v99[2]] = v75[v99[3]];
											v91 = v91 + 1;
											v99 = v87[v91];
											v97[v99[2]] = v99[3];
											v91 = v91 + 1;
											v99 = v87[v91];
											v153 = v99[2];
											v97[v153] = v97[v153](v97[v153 + 1]);
											v91 = v91 + 1;
											v99 = v87[v91];
											v97[v99[2]] = v75[v99[3]];
											v91 = v91 + 1;
											v99 = v87[v91];
											v97[v99[2]] = v97[v99[3 + 0]];
											v91 = v91 + 1;
											v99 = v87[v91];
											v153 = v99[2];
											v152 = {v97[v153](v97[v153 + 1])};
											v151 = 0;
											for v316 = v153, v99[9 - 5] do
												local v317 = 0;
												while true do
													if (0 == v317) then
														v151 = v151 + 1 + 0;
														v97[v316] = v152[v151];
														break;
													end
												end
											end
											v91 = v91 + 1;
											v99 = v87[v91];
											v91 = v99[3];
										end
									elseif (v100 <= 4) then
										if (v100 == 3) then
											if (v97[v99[7 - 5]] == v99[956 - (802 + 150)]) then
												v91 = v91 + (2 - 1);
											else
												v91 = v99[3];
											end
										else
											v97[v99[2]] = v40(v88[v99[3]], nil, v75);
										end
									elseif (v100 == 5) then
										local v162 = 0;
										local v163;
										while true do
											if (v162 == 0) then
												v163 = v99[2];
												do
													return v21(v97, v163, v163 + v99[3]);
												end
												break;
											end
										end
									else
										v97[v99[3 - 1]] = v97[v99[3]];
									end
								elseif (v100 <= 10) then
									if (v100 <= 8) then
										if (v100 > 7) then
											v97[v99[2]] = v97[v99[3]] * v97[v99[3 + 1]];
										else
											local v167 = 0;
											local v168;
											local v169;
											local v170;
											while true do
												if (v167 == 1) then
													v170 = 0;
													for v554 = v168, v99[11 - 7] do
														v170 = v170 + 1;
														v97[v554] = v169[v170];
													end
													break;
												end
												if (0 == v167) then
													v168 = v99[2];
													v169 = {v97[v168](v97[v168 + 1])};
													v167 = 1;
												end
											end
										end
									elseif (v100 == 9) then
										if (v97[v99[2]] < v97[v99[4]]) then
											v91 = v91 + 1;
										else
											v91 = v99[3];
										end
									else
										local v171 = 0;
										while true do
											if (3 == v171) then
												v97[v99[2]] = v75[v99[3]];
												v91 = v91 + 1;
												v99 = v87[v91];
												v97[v99[2]] = v97[v99[3]][v99[4 - 0]];
												v171 = 4;
											end
											if (v171 == 1) then
												v91 = v91 + 1;
												v99 = v87[v91];
												v97[v99[2 + 0]] = v75[v99[3]];
												v91 = v91 + 1;
												v171 = 2;
											end
											if (v171 == 2) then
												v99 = v87[v91];
												v97[v99[2]] = v97[v99[3]][v99[4]];
												v91 = v91 + 1;
												v99 = v87[v91];
												v171 = 3;
											end
											if (v171 == 4) then
												v91 = v91 + 1;
												v99 = v87[v91];
												v97[v99[2]] = v75[v99[3]];
												v91 = v91 + 1;
												v171 = 5;
											end
											if (v171 == 5) then
												v99 = v87[v91];
												if not v97[v99[2]] then
													v91 = v91 + (1188 - (1069 + 118));
												else
													v91 = v99[3];
												end
												break;
											end
											if (v171 == 0) then
												v97[v99[2]] = v75[v99[3]];
												v91 = v91 + 1;
												v99 = v87[v91];
												v97[v99[2]] = v97[v99[3]][v99[4]];
												v171 = 1;
											end
										end
									end
								elseif (v100 <= 12) then
									if (v100 == 11) then
										v97[v99[2]] = v97[v99[3]] % v97[v99[4]];
									else
										local v173 = 0;
										local v174;
										local v175;
										local v176;
										local v177;
										local v178;
										local v179;
										while true do
											if (v173 == 3) then
												v91 = v91 + (1 - 0);
												v99 = v87[v91];
												v97[v99[2]] = v97[v99[3]][v99[4]];
												v91 = v91 + 1;
												v173 = 4;
											end
											if (v173 == 6) then
												for v557 = v179, v92 do
													local v558 = 0;
													while true do
														if (v558 == 0) then
															v176 = v176 + 1;
															v97[v557] = v177[v176];
															break;
														end
													end
												end
												v91 = v91 + 1 + 0;
												v99 = v87[v91];
												v179 = v99[2];
												v173 = 7;
											end
											if (v173 == 7) then
												v97[v179] = v97[v179](v21(v97, v179 + 1, v92));
												v91 = v91 + 1;
												v99 = v87[v91];
												v97[v99[2]] = v99[3];
												v173 = 8;
											end
											if (v173 == 0) then
												v174 = nil;
												v175 = nil;
												v176 = nil;
												v177, v178 = nil;
												v173 = 1;
											end
											if (v173 == 4) then
												v99 = v87[v91];
												v97[v99[1 + 1]] = v97[v99[3]];
												v91 = v91 + 1;
												v99 = v87[v91];
												v173 = 5;
											end
											if (2 == v173) then
												v97[v99[2]] = v97[v99[3]][v99[8 - 4]];
												v91 = v91 + 1;
												v99 = v87[v91];
												v97[v99[2]] = v75[v99[3]];
												v173 = 3;
											end
											if (v173 == 9) then
												v174 = v97[v179 + 2];
												if (v174 > 0) then
													if (v175 > v97[v179 + 1]) then
														v91 = v99[3];
													else
														v97[v179 + 3] = v175;
													end
												elseif (v175 < v97[v179 + 1]) then
													v91 = v99[3];
												else
													v97[v179 + 3] = v175;
												end
												break;
											end
											if (v173 == 5) then
												v179 = v99[2];
												v177, v178 = v90(v97[v179](v97[v179 + (1 - 0)]));
												v92 = (v178 + v179) - 1;
												v176 = 0;
												v173 = 6;
											end
											if (v173 == 1) then
												v179 = nil;
												v97[v99[2]] = v75[v99[3]];
												v91 = v91 + 1;
												v99 = v87[v91];
												v173 = 2;
											end
											if (v173 == 8) then
												v91 = v91 + (792 - (368 + 423));
												v99 = v87[v91];
												v179 = v99[2];
												v175 = v97[v179];
												v173 = 9;
											end
										end
									end
								elseif (v100 > 13) then
									local v180 = 0;
									local v181;
									local v182;
									local v183;
									local v184;
									while true do
										if (v180 == 1) then
											v92 = (v183 + v181) - 1;
											v184 = 0;
											v180 = 2;
										end
										if (v180 == 2) then
											for v559 = v181, v92 do
												local v560 = 0;
												while true do
													if (v560 == 0) then
														v184 = v184 + 1;
														v97[v559] = v182[v184];
														break;
													end
												end
											end
											break;
										end
										if (v180 == 0) then
											v181 = v99[2];
											v182, v183 = v90(v97[v181](v21(v97, v181 + 1, v99[3])));
											v180 = 1;
										end
									end
								else
									v91 = v99[3];
								end
							elseif (v100 <= (65 - 44)) then
								if (v100 <= 17) then
									if (v100 <= (33 - (10 + 8))) then
										v97[v99[2]] = {};
									elseif (v100 > 16) then
										v97[v99[2]] = v75[v99[3]];
									else
										v97[v99[2]] = v97[v99[3]] + v99[4];
									end
								elseif (v100 <= 19) then
									if (v100 == 18) then
										if (v99[2] == v97[v99[4]]) then
											v91 = v91 + 1;
										else
											v91 = v99[3];
										end
									else
										local v189 = v99[2];
										local v190 = v99[15 - 11];
										local v191 = v189 + 2;
										local v192 = {v97[v189](v97[v189 + 1], v97[v191])};
										for v318 = 1, v190 do
											v97[v191 + v318] = v192[v318];
										end
										local v193 = v192[1];
										if v193 then
											local v333 = 0;
											while true do
												if (0 == v333) then
													v97[v191] = v193;
													v91 = v99[3];
													break;
												end
											end
										else
											v91 = v91 + 1;
										end
									end
								elseif (v100 == 20) then
									if v97[v99[2]] then
										v91 = v91 + (443 - (416 + 26));
									else
										v91 = v99[3];
									end
								else
									local v194 = 0;
									local v195;
									local v196;
									local v197;
									while true do
										if (v194 == 0) then
											v195 = v99[2];
											v196 = v97[v195];
											v194 = 1;
										end
										if (v194 == 1) then
											v197 = v97[v195 + 2];
											if (v197 > 0) then
												if (v196 > v97[v195 + 1]) then
													v91 = v99[3];
												else
													v97[v195 + 3] = v196;
												end
											elseif (v196 < v97[v195 + 1]) then
												v91 = v99[3];
											else
												v97[v195 + 3] = v196;
											end
											break;
										end
									end
								end
							elseif (v100 <= 25) then
								if (v100 <= 23) then
									if (v100 == 22) then
										v97[v99[2]] = #v97[v99[3]];
									else
										local v199 = 0;
										local v200;
										while true do
											if (v199 == 0) then
												v200 = v99[2];
												do
													return v97[v200](v21(v97, v200 + 1, v99[3]));
												end
												break;
											end
										end
									end
								elseif (v100 == 24) then
									local v201 = 0;
									local v202;
									while true do
										if (v201 == 0) then
											v202 = v99[6 - 4];
											v97[v202] = v97[v202](v21(v97, v202 + 1, v99[3]));
											break;
										end
									end
								else
									local v203 = v99[2];
									local v204, v205 = v90(v97[v203](v97[v203 + 1 + 0]));
									v92 = (v205 + v203) - 1;
									local v206 = 0;
									for v321 = v203, v92 do
										local v322 = 0;
										while true do
											if (v322 == 0) then
												v206 = v206 + 1;
												v97[v321] = v204[v206];
												break;
											end
										end
									end
								end
							elseif (v100 <= 27) then
								if (v100 == 26) then
									v97[v99[2]] = v97[v99[3]][v99[4]];
								else
									v97[v99[2]] = v99[4 - 1] + v97[v99[4]];
								end
							elseif (v100 > 28) then
								v97[v99[2]] = v74[v99[3]];
							else
								local v212 = 0;
								local v213;
								local v214;
								local v215;
								while true do
									if (v212 == 4) then
										v214 = v97[v215];
										v213 = v97[v215 + 2];
										if (v213 > 0) then
											if (v214 > v97[v215 + 1]) then
												v91 = v99[1489 - (998 + 488)];
											else
												v97[v215 + 1 + 2] = v214;
											end
										elseif (v214 < v97[v215 + 1]) then
											v91 = v99[3];
										else
											v97[v215 + 3] = v214;
										end
										break;
									end
									if (v212 == 1) then
										v91 = v91 + 1;
										v99 = v87[v91];
										v97[v99[2]] = v99[3];
										v91 = v91 + 1;
										v212 = 2;
									end
									if (2 == v212) then
										v99 = v87[v91];
										v97[v99[440 - (145 + 293)]] = #v97[v99[3]];
										v91 = v91 + (431 - (44 + 386));
										v99 = v87[v91];
										v212 = 3;
									end
									if (v212 == 0) then
										v213 = nil;
										v214 = nil;
										v215 = nil;
										v97[v99[2]] = {};
										v212 = 1;
									end
									if (v212 == 3) then
										v97[v99[2]] = v99[3];
										v91 = v91 + 1;
										v99 = v87[v91];
										v215 = v99[2];
										v212 = 4;
									end
								end
							end
						elseif (v100 <= 44) then
							if (v100 <= 36) then
								if (v100 <= 32) then
									if (v100 <= 30) then
										local v145 = 0;
										local v146;
										while true do
											if (v145 == 0) then
												v146 = v99[2];
												v97[v146](v97[v146 + 1]);
												break;
											end
										end
									elseif (v100 == 31) then
										local v216 = 0;
										local v217;
										while true do
											if (v216 == 0) then
												v217 = v99[2];
												v97[v217](v21(v97, v217 + 1 + 0, v92));
												break;
											end
										end
									else
										for v324 = v99[2], v99[3] do
											v97[v324] = nil;
										end
									end
								elseif (v100 <= 34) then
									if (v100 == 33) then
										v75[v99[3]] = v97[v99[774 - (201 + 571)]];
									else
										v97[v99[2]] = v97[v99[3]] + v99[4];
										v91 = v91 + 1;
										v99 = v87[v91];
										v97[v99[1140 - (116 + 1022)]] = v97[v99[3]] + v99[4];
										v91 = v91 + 1;
										v99 = v87[v91];
										v97[v99[2]] = v99[12 - 9];
										v91 = v91 + 1;
										v99 = v87[v91];
										v97[v99[2]] = v99[3];
										v91 = v91 + 1;
										v99 = v87[v91];
										v97[v99[2 + 0]] = v99[3];
										v91 = v91 + 1;
										v99 = v87[v91];
										if (v97[v99[2]] < v97[v99[4]]) then
											v91 = v91 + 1;
										else
											v91 = v99[3];
										end
									end
								elseif (v100 == 35) then
									local v226 = 0;
									local v227;
									local v228;
									local v229;
									local v230;
									while true do
										if (v226 == 2) then
											v97[v99[2]] = v74[v99[3]];
											v91 = v91 + (860 - (814 + 45));
											v99 = v87[v91];
											v97[v99[2]] = v74[v99[3]];
											v91 = v91 + (2 - 1);
											v99 = v87[v91];
											v226 = 3;
										end
										if (v226 == 6) then
											v91 = v91 + 1;
											v99 = v87[v91];
											v97[v99[2]] = v74[v99[3]];
											v91 = v91 + 1;
											v99 = v87[v91];
											v97[v99[2]] = v74[v99[3]];
											v226 = 7;
										end
										if (v226 == 8) then
											v91 = v91 + 1;
											v99 = v87[v91];
											v97[v99[2]] = v97[v99[3]] % v97[v99[4]];
											v91 = v91 + 1;
											v99 = v87[v91];
											v97[v99[2]] = v99[3] + v97[v99[4]];
											v226 = 9;
										end
										if (v226 == 0) then
											v227 = nil;
											v228, v229 = nil;
											v230 = nil;
											v97[v99[2]] = v97[v99[3]];
											v91 = v91 + 1;
											v99 = v87[v91];
											v226 = 1;
										end
										if (v226 == 9) then
											v91 = v91 + 1;
											v99 = v87[v91];
											v97[v99[887 - (261 + 624)]] = #v97[v99[3]];
											v91 = v91 + 1;
											v99 = v87[v91];
											v97[v99[2]] = v97[v99[3]] % v97[v99[4]];
											v226 = 10;
										end
										if (v226 == 16) then
											v230 = v99[2];
											v97[v230](v21(v97, v230 + 1, v92));
											break;
										end
										if (v226 == 7) then
											v91 = v91 + 1;
											v99 = v87[v91];
											v97[v99[2]] = v97[v99[3]];
											v91 = v91 + 1 + 0;
											v99 = v87[v91];
											v97[v99[2]] = #v97[v99[3]];
											v226 = 8;
										end
										if (13 == v226) then
											v227 = 0;
											for v563 = v230, v92 do
												local v564 = 0;
												while true do
													if (v564 == 0) then
														v227 = v227 + 1;
														v97[v563] = v228[v227];
														break;
													end
												end
											end
											v91 = v91 + 1;
											v99 = v87[v91];
											v230 = v99[2];
											v97[v230] = v97[v230](v21(v97, v230 + (1 - 0), v92));
											v226 = 14;
										end
										if (v226 == 15) then
											v228, v229 = v90(v97[v230](v97[v230 + 1]));
											v92 = (v229 + v230) - 1;
											v227 = 0;
											for v565 = v230, v92 do
												local v566 = 0;
												while true do
													if (0 == v566) then
														v227 = v227 + (1081 - (1020 + 60));
														v97[v565] = v228[v227];
														break;
													end
												end
											end
											v91 = v91 + 1;
											v99 = v87[v91];
											v226 = 16;
										end
										if (v226 == 14) then
											v91 = v91 + 1;
											v99 = v87[v91];
											v97[v99[2]] = v97[v99[3]] % v99[4];
											v91 = v91 + 1;
											v99 = v87[v91];
											v230 = v99[2];
											v226 = 15;
										end
										if (v226 == 5) then
											v227 = 0;
											for v567 = v230, v92 do
												local v568 = 0;
												while true do
													if (0 == v568) then
														v227 = v227 + 1;
														v97[v567] = v228[v227];
														break;
													end
												end
											end
											v91 = v91 + 1;
											v99 = v87[v91];
											v230 = v99[2];
											v97[v230] = v97[v230](v21(v97, v230 + 1, v92));
											v226 = 6;
										end
										if (v226 == 3) then
											v97[v99[2]] = v97[v99[3]];
											v91 = v91 + 1;
											v99 = v87[v91];
											v97[v99[2]] = v97[v99[3]];
											v91 = v91 + 1;
											v99 = v87[v91];
											v226 = 4;
										end
										if (v226 == 12) then
											for v569 = v230, v92 do
												local v570 = 0;
												while true do
													if (v570 == 0) then
														v227 = v227 + 1;
														v97[v569] = v228[v227];
														break;
													end
												end
											end
											v91 = v91 + 1;
											v99 = v87[v91];
											v230 = v99[2];
											v228, v229 = v90(v97[v230](v21(v97, v230 + 1, v92)));
											v92 = (v229 + v230) - 1;
											v226 = 13;
										end
										if (v226 == 10) then
											v91 = v91 + 1;
											v99 = v87[v91];
											v97[v99[2]] = v99[3] + v97[v99[4]];
											v91 = v91 + 1;
											v99 = v87[v91];
											v97[v99[2]] = v97[v99[3]] + v99[4];
											v226 = 11;
										end
										if (v226 == 4) then
											v97[v99[2]] = v97[v99[1 + 2]] + v99[4];
											v91 = v91 + 1;
											v99 = v87[v91];
											v230 = v99[2];
											v228, v229 = v90(v97[v230](v21(v97, v230 + 1, v99[3])));
											v92 = (v229 + v230) - 1;
											v226 = 5;
										end
										if (1 == v226) then
											v97[v99[2]] = v74[v99[3]];
											v91 = v91 + (3 - 2);
											v99 = v87[v91];
											v97[v99[2]] = v74[v99[10 - 7]];
											v91 = v91 + 1;
											v99 = v87[v91];
											v226 = 2;
										end
										if (v226 == 11) then
											v91 = v91 + 1;
											v99 = v87[v91];
											v230 = v99[2];
											v228, v229 = v90(v97[v230](v21(v97, v230 + 1, v99[3])));
											v92 = (v229 + v230) - 1;
											v227 = 0;
											v226 = 12;
										end
									end
								else
									local v231 = 0;
									local v232;
									local v233;
									while true do
										if (v231 == 0) then
											v232 = v99[2];
											v233 = v97[v232];
											v231 = 1;
										end
										if (v231 == 1) then
											for v571 = v232 + 1, v92 do
												v15(v233, v97[v571]);
											end
											break;
										end
									end
								end
							elseif (v100 <= 40) then
								if (v100 <= 38) then
									if (v100 == (1460 - (630 + 793))) then
										v97[v99[2]] = v99[9 - 6];
									else
										local v236 = 0;
										local v237;
										local v238;
										local v239;
										while true do
											if (v236 == 0) then
												v237 = nil;
												v238 = nil;
												v239 = nil;
												v236 = 1;
											end
											if (v236 == 5) then
												v239 = v99[2];
												v238 = v97[v239];
												v237 = v97[v239 + 2];
												v236 = 6;
											end
											if (v236 == 1) then
												v97[v99[9 - 7]] = v97[v99[3]];
												v91 = v91 + 1;
												v99 = v87[v91];
												v236 = 2;
											end
											if (v236 == 6) then
												if (v237 > (0 - 0)) then
													if (v238 > v97[v239 + 1]) then
														v91 = v99[1750 - (760 + 987)];
													else
														v97[v239 + (1916 - (1789 + 124))] = v238;
													end
												elseif (v238 < v97[v239 + 1]) then
													v91 = v99[769 - (745 + 21)];
												else
													v97[v239 + 3] = v238;
												end
												break;
											end
											if (v236 == 3) then
												v97[v99[1 + 1]] = v97[v99[3]];
												v91 = v91 + 1;
												v99 = v87[v91];
												v236 = 4;
											end
											if (v236 == 2) then
												v97[v99[2]] = v99[3];
												v91 = v91 + 1;
												v99 = v87[v91];
												v236 = 3;
											end
											if (v236 == 4) then
												v97[v99[2]] = v99[3];
												v91 = v91 + 1;
												v99 = v87[v91];
												v236 = 5;
											end
										end
									end
								elseif (v100 > 39) then
									local v240 = 0;
									local v241;
									local v242;
									local v243;
									while true do
										if (v240 == 1) then
											v243 = v97[v241] + v242;
											v97[v241] = v243;
											v240 = 2;
										end
										if (2 == v240) then
											if (v242 > 0) then
												if (v243 <= v97[v241 + 1]) then
													v91 = v99[3];
													v97[v241 + 2 + 1] = v243;
												end
											elseif (v243 >= v97[v241 + 1]) then
												local v639 = 0;
												while true do
													if (0 == v639) then
														v91 = v99[7 - 4];
														v97[v241 + 3] = v243;
														break;
													end
												end
											end
											break;
										end
										if (v240 == 0) then
											v241 = v99[2];
											v242 = v97[v241 + 2];
											v240 = 1;
										end
									end
								elseif not v97[v99[2]] then
									v91 = v91 + 1;
								else
									v91 = v99[3];
								end
							elseif (v100 <= 42) then
								if (v100 > 41) then
									local v244 = 0;
									local v245;
									local v246;
									while true do
										if (v244 == 1) then
											for v572 = v245 + (3 - 2), v99[4] do
												v246 = v246 .. v97[v572];
											end
											v97[v99[2]] = v246;
											break;
										end
										if (v244 == 0) then
											v245 = v99[3];
											v246 = v97[v245];
											v244 = 1;
										end
									end
								else
									v97[v99[2]][v97[v99[3]]] = v99[4];
								end
							elseif (v100 > 43) then
								local v249 = 0;
								local v250;
								local v251;
								local v252;
								while true do
									if (2 == v249) then
										for v573 = 1, v99[4] do
											local v574 = 0;
											local v575;
											while true do
												if (v574 == 0) then
													v91 = v91 + 1;
													v575 = v87[v91];
													v574 = 1;
												end
												if (v574 == 1) then
													if (v575[1] == 6) then
														v252[v573 - 1] = {v97,v575[3]};
													else
														v252[v573 - 1] = {v74,v575[3]};
													end
													v96[#v96 + 1] = v252;
													break;
												end
											end
										end
										v97[v99[2]] = v40(v250, v251, v75);
										break;
									end
									if (v249 == 1) then
										v252 = {};
										v251 = v18({}, {[v7("\69\131\167\225\218\127\164", "\190\26\220\206\143")]=function(v576, v577)
											local v578 = v252[v577];
											return v578[1][v578[2]];
										end,[v7("\237\185\115\40\0\209\194\193\215\158", "\165\178\230\29\77\119\184\172")]=function(v579, v580, v581)
											local v582 = v252[v580];
											v582[1][v582[2]] = v581;
										end});
										v249 = 2;
									end
									if (v249 == 0) then
										v250 = v88[v99[3]];
										v251 = nil;
										v249 = 1;
									end
								end
							else
								do
									return v97[v99[2]];
								end
							end
						elseif (v100 <= 52) then
							if (v100 <= 48) then
								if (v100 <= (37 + 9)) then
									if (v100 == 45) then
										local v253 = 0;
										local v254;
										local v255;
										local v256;
										local v257;
										while true do
											if (v253 == 0) then
												v254 = nil;
												v255, v256 = nil;
												v257 = nil;
												v97[v99[2]] = v74[v99[3]];
												v253 = 1;
											end
											if (v253 == 5) then
												v97[v257](v21(v97, v257 + 1, v92));
												v91 = v91 + 1;
												v99 = v87[v91];
												v91 = v99[3];
												break;
											end
											if (v253 == 4) then
												for v584 = v257, v92 do
													v254 = v254 + 1;
													v97[v584] = v255[v254];
												end
												v91 = v91 + (1056 - (87 + 968));
												v99 = v87[v91];
												v257 = v99[2];
												v253 = 5;
											end
											if (v253 == 2) then
												v99 = v87[v91];
												v97[v99[2]] = v99[3];
												v91 = v91 + 1;
												v99 = v87[v91];
												v253 = 3;
											end
											if (v253 == 3) then
												v257 = v99[2];
												v255, v256 = v90(v97[v257](v21(v97, v257 + 1, v99[3])));
												v92 = (v256 + v257) - 1;
												v254 = 0;
												v253 = 4;
											end
											if (v253 == 1) then
												v91 = v91 + 1;
												v99 = v87[v91];
												v97[v99[2]] = v99[3];
												v91 = v91 + 1;
												v253 = 2;
											end
										end
									else
										v97[v99[2]] = v99[3] ~= (0 - 0);
									end
								elseif (v100 == 47) then
									local v259 = 0;
									local v260;
									while true do
										if (0 == v259) then
											v260 = v99[2];
											v97[v260] = v97[v260](v21(v97, v260 + 1, v92));
											break;
										end
									end
								else
									local v261 = 0;
									while true do
										if (0 == v261) then
											v97[v99[2]] = v99[3] ~= 0;
											v91 = v91 + 1;
											break;
										end
									end
								end
							elseif (v100 <= 50) then
								if (v100 > 49) then
									local v262 = 0;
									local v263;
									local v264;
									local v265;
									local v266;
									while true do
										if (1 == v262) then
											v91 = v91 + 1;
											v99 = v87[v91];
											v97[v99[2]] = v99[3];
											v91 = v91 + 1;
											v262 = 2;
										end
										if (v262 == 2) then
											v99 = v87[v91];
											v97[v99[2]] = v99[3 + 0];
											v91 = v91 + 1;
											v99 = v87[v91];
											v262 = 3;
										end
										if (v262 == 3) then
											v266 = v99[2];
											v264, v265 = v90(v97[v266](v21(v97, v266 + (2 - 1), v99[3])));
											v92 = (v265 + v266) - 1;
											v263 = 0;
											v262 = 4;
										end
										if (v262 == 5) then
											v97[v266](v21(v97, v266 + 1, v92));
											break;
										end
										if (v262 == 0) then
											v263 = nil;
											v264, v265 = nil;
											v266 = nil;
											v97[v99[2]] = v74[v99[3]];
											v262 = 1;
										end
										if (4 == v262) then
											for v587 = v266, v92 do
												local v588 = 0;
												while true do
													if (0 == v588) then
														v263 = v263 + 1;
														v97[v587] = v264[v263];
														break;
													end
												end
											end
											v91 = v91 + 1;
											v99 = v87[v91];
											v266 = v99[1415 - (447 + 966)];
											v262 = 5;
										end
									end
								else
									v97[v99[2]] = v97[v99[8 - 5]][v97[v99[4]]];
								end
							elseif (v100 > 51) then
								local v269 = 0;
								local v270;
								while true do
									if (v269 == 0) then
										v270 = v99[2];
										v97[v270] = v97[v270](v97[v270 + 1]);
										break;
									end
								end
							else
								local v271 = 0;
								local v272;
								local v273;
								local v274;
								local v275;
								local v276;
								while true do
									if (v271 == 3) then
										v99 = v87[v91];
										v97[v99[2]] = v97[v99[3]];
										v91 = v91 + 1;
										v99 = v87[v91];
										for v589 = v99[2], v99[3] do
											v97[v589] = nil;
										end
										v91 = v91 + 1;
										v271 = 4;
									end
									if (v271 == 2) then
										v99 = v87[v91];
										v97[v99[2]] = {};
										v91 = v91 + 1;
										v99 = v87[v91];
										v97[v99[703 - (376 + 325)]] = v74[v99[3]];
										v91 = v91 + 1;
										v271 = 3;
									end
									if (v271 == 5) then
										v91 = v91 + (1 - 0);
										v99 = v87[v91];
										v276 = v99[5 - 3];
										v272 = v97[v276];
										for v591 = v276 + 1, v92 do
											v15(v272, v97[v591]);
										end
										break;
									end
									if (v271 == 4) then
										v99 = v87[v91];
										v276 = v99[2];
										v274, v275 = v90(v97[v276](v21(v97, v276 + 1, v99[3])));
										v92 = (v275 + v276) - 1;
										v273 = 0;
										for v592 = v276, v92 do
											v273 = v273 + 1;
											v97[v592] = v274[v273];
										end
										v271 = 5;
									end
									if (v271 == 0) then
										v272 = nil;
										v273 = nil;
										v274, v275 = nil;
										v276 = nil;
										v97[v99[1819 - (1703 + 114)]] = v74[v99[3]];
										v91 = v91 + 1;
										v271 = 1;
									end
									if (v271 == 1) then
										v99 = v87[v91];
										v97[v99[2]] = v74[v99[3]];
										v91 = v91 + 1;
										v99 = v87[v91];
										v97[v99[2]] = v74[v99[3]];
										v91 = v91 + 1;
										v271 = 2;
									end
								end
							end
						elseif (v100 <= (17 + 39)) then
							if (v100 <= 54) then
								if (v100 > 53) then
									local v277 = 0;
									local v278;
									while true do
										if (0 == v277) then
											v278 = v99[2];
											do
												return v21(v97, v278, v92);
											end
											break;
										end
									end
								else
									v97[v99[2]] = v97[v99[3]] % v99[4];
								end
							elseif (v100 == 55) then
								do
									return;
								end
							else
								do
									return v97[v99[4 - 2]]();
								end
							end
						elseif (v100 <= 58) then
							if (v100 == 57) then
								local v280 = 0;
								local v281;
								local v282;
								local v283;
								local v284;
								while true do
									if (0 == v280) then
										v281 = nil;
										v282, v283 = nil;
										v284 = nil;
										v97[v99[2]] = v99[3];
										v280 = 1;
									end
									if (v280 == 2) then
										v91 = v91 + 1;
										v99 = v87[v91];
										v97[v99[2]] = v99[3];
										v91 = v91 + 1;
										v280 = 3;
									end
									if (v280 == 5) then
										v284 = v99[1267 - (243 + 1022)];
										v97[v284] = v97[v284](v21(v97, v284 + (3 - 2), v92));
										v91 = v91 + 1 + 0;
										v99 = v87[v91];
										v280 = 6;
									end
									if (v280 == 1) then
										v91 = v91 + 1;
										v99 = v87[v91];
										v284 = v99[16 - (9 + 5)];
										v97[v284] = v97[v284](v21(v97, v284 + 1, v99[3]));
										v280 = 2;
									end
									if (4 == v280) then
										v281 = 376 - (85 + 291);
										for v595 = v284, v92 do
											v281 = v281 + 1;
											v97[v595] = v282[v281];
										end
										v91 = v91 + 1;
										v99 = v87[v91];
										v280 = 5;
									end
									if (3 == v280) then
										v99 = v87[v91];
										v284 = v99[2];
										v282, v283 = v90(v97[v284](v21(v97, v284 + 1, v99[3])));
										v92 = (v283 + v284) - 1;
										v280 = 4;
									end
									if (6 == v280) then
										if (v97[v99[2]] == v99[4]) then
											v91 = v91 + 1;
										else
											v91 = v99[3];
										end
										break;
									end
								end
							else
								local v285;
								local v286, v287;
								local v288;
								v97[v99[2]] = v74[v99[1183 - (1123 + 57)]];
								v91 = v91 + 1;
								v99 = v87[v91];
								v97[v99[2 + 0]] = v99[3];
								v91 = v91 + 1;
								v99 = v87[v91];
								v97[v99[2]] = v99[257 - (163 + 91)];
								v91 = v91 + 1;
								v99 = v87[v91];
								v288 = v99[2];
								v286, v287 = v90(v97[v288](v21(v97, v288 + (1931 - (1869 + 61)), v99[3])));
								v92 = (v287 + v288) - 1;
								v285 = 0;
								for v326 = v288, v92 do
									local v327 = 0;
									while true do
										if (v327 == 0) then
											v285 = v285 + 1;
											v97[v326] = v286[v285];
											break;
										end
									end
								end
								v91 = v91 + 1 + 0;
								v99 = v87[v91];
								v288 = v99[2];
								v97[v288](v21(v97, v288 + 1, v92));
							end
						elseif (v100 > 59) then
							local v296 = 0;
							local v297;
							local v298;
							local v299;
							while true do
								if (v296 == 1) then
									v97[v99[2]] = v74[v99[3]];
									v91 = v91 + 1;
									v99 = v87[v91];
									v296 = 2;
								end
								if (2 == v296) then
									v97[v99[2]] = v99[10 - 7];
									v91 = v91 + 1;
									v99 = v87[v91];
									v296 = 3;
								end
								if (v296 == 7) then
									for v600 = v298 + 1, v99[4] do
										v297 = v297 .. v97[v600];
									end
									v97[v99[2]] = v297;
									v91 = v91 + 1;
									v296 = 8;
								end
								if (6 == v296) then
									v99 = v87[v91];
									v298 = v99[3];
									v297 = v97[v298];
									v296 = 7;
								end
								if (v296 == 0) then
									v297 = nil;
									v298 = nil;
									v299 = nil;
									v296 = 1;
								end
								if (v296 == 4) then
									v299 = v99[2];
									v97[v299] = v97[v299](v21(v97, v299 + 1, v99[3]));
									v91 = v91 + 1;
									v296 = 5;
								end
								if (v296 == 3) then
									v97[v99[2]] = v99[4 - 1];
									v91 = v91 + 1;
									v99 = v87[v91];
									v296 = 4;
								end
								if (8 == v296) then
									v99 = v87[v91];
									v299 = v99[2];
									v97[v299](v97[v299 + 1]);
									break;
								end
								if (v296 == 5) then
									v99 = v87[v91];
									v97[v99[2]] = v97[v99[3]];
									v91 = v91 + 1;
									v296 = 6;
								end
							end
						else
							local v300 = 0;
							local v301;
							local v302;
							local v303;
							local v304;
							while true do
								if (v300 == 2) then
									for v601 = v301, v92 do
										local v602 = 0;
										while true do
											if (v602 == 0) then
												v304 = v304 + 1;
												v97[v601] = v302[v304];
												break;
											end
										end
									end
									break;
								end
								if (v300 == 0) then
									v301 = v99[1 + 1];
									v302, v303 = v90(v97[v301](v21(v97, v301 + 1, v92)));
									v300 = 1;
								end
								if (v300 == 1) then
									v92 = (v303 + v301) - 1;
									v304 = 0;
									v300 = 2;
								end
							end
						end
						v91 = v91 + 1;
						break;
					end
				end
			end
		end;
	end
	return v40(v39(), {}, v28)(...);
end
return v23("LOL!0D3Q0003063Q00737472696E6703043Q006368617203043Q00627974652Q033Q0073756203053Q0062697433322Q033Q0062697403043Q0062786F7203053Q007461626C6503063Q00636F6E63617403063Q00696E7365727403053Q006D6174636803083Q00746F6E756D62657203053Q007063612Q6C00243Q00120A3Q00013Q00206Q000200122Q000100013Q00202Q00010001000300122Q000200013Q00202Q00020002000400122Q000300053Q00062Q0003000A0001000100040D3Q000A0001001211000300063Q00201A000400030007001211000500083Q00201A000500050009001211000600083Q00201A00060006000A00062C00073Q000100062Q00063Q00064Q00068Q00063Q00044Q00063Q00014Q00063Q00024Q00063Q00053Q001211000800013Q00201A00080008000B0012110009000C3Q001211000A000D3Q00062C000B0001000100052Q00063Q00074Q00063Q00094Q00063Q00084Q00063Q000A4Q00063Q000B4Q0006000C000B4Q0038000C00014Q0036000C6Q00373Q00013Q00023Q00023Q00026Q00F03F026Q00704002264Q001C00025Q00122Q000300016Q00045Q00122Q000500013Q00042Q0003002100012Q001D00076Q0023000800026Q000900016Q000A00026Q000B00036Q000C00046Q000D8Q000E00063Q00202Q000F000600014Q000C000F6Q000B3Q00024Q000C00036Q000D00046Q000E00016Q000F00016Q000F0006000F00102Q000F0001000F4Q001000016Q00100006001000102Q00100001001000202Q0010001000014Q000D00106Q000C8Q000A3Q000200202Q000A000A00024Q0009000A6Q00073Q00010004280003000500012Q001D000300054Q0006000400024Q0017000300044Q003600036Q00373Q00017Q00043Q00027Q004003053Q003A25642B3A2Q033Q0025642B026Q00F03F001C3Q00062C5Q000100012Q001D8Q0033000100016Q000200026Q000300026Q00048Q000500036Q00068Q000700076Q000500076Q00043Q000100201A000400040001001239000500026Q00030005000200122Q000400036Q000200046Q00013Q000200262Q000100180001000400040D3Q001800012Q000600016Q000F00026Q0017000100024Q003600015Q00040D3Q001B00012Q001D000100044Q0038000100014Q003600016Q00373Q00013Q00013Q00153Q00024Q00F0E4FD40026Q003440025Q00C05940025Q005D3241024Q0087C63241023Q00406E9B5E4103053Q007072696E7403043Q0002AE332B03083Q002976DC464E9E3076026Q00F03F03193Q00D9F9AD3101D5FABF2152C2F3AE6411D9F5AF2D06DFF4A5375303053Q0072B69BCB4403343Q0050A9B7FB4D3F7DA2FEC3752261ACB0FF550B33B2B7F44A7670AAB3E84A3367A0B2E1063E7AA1BBB8523E7AB6FEEB52247AAB2QB903063Q005613C5DE982603153Q0073696576655F6F665F657261746F737468656E6573025Q00407A4003053Q007061697273030D3Q00CC5271E8780630F35576E1270603073Q00569C2018851D2603163Q008F8A54E8697317A88745BD6E7F56B38003AA786F43F803073Q0037C7E523C81D1C013D3Q0006143Q003B00013Q00040D3Q003B0001001225000100013Q00202200020001000200202Q00010002000300122Q000200043Q00122Q000300053Q00122Q000400063Q00062Q000200100001000300040D3Q00100001001211000500074Q003200065Q00122Q000700083Q00122Q000800096Q000600086Q00053Q000100101B0005000A0004000609000300190001000500040D3Q00190001001211000500074Q003200065Q00122Q0007000B3Q00122Q0008000C6Q000600086Q00053Q0001001211000500074Q003200065Q00122Q0007000D3Q00122Q0008000E6Q000600086Q00053Q000100020400055Q0012020005000F3Q00122Q0005000F3Q00122Q000600106Q00050002000200122Q000600116Q000700056Q00060002000800044Q00320001000614000A003200013Q00040D3Q00320001001211000B00074Q003C000C5Q00122Q000D00123Q00122Q000E00136Q000C000E00024Q000D00096Q000C000C000D4Q000B00020001000613000600280001000200040D3Q00280001001211000500074Q003200065Q00122Q000700143Q00122Q000800156Q000600086Q00053Q000100040D3Q003C000100201A00013Q000A2Q00373Q00013Q00013Q00073Q00028Q00026Q00F03F027Q004003043Q006D61746803053Q00666C2Q6F7203043Q00737172740100013F3Q001225000100014Q0020000200033Q002603000200380001000200040D3Q003800010026030002001F0001000200040D3Q001F0001001225000400013Q002603000400070001000100040D3Q00070001001225000500033Q00120C000600043Q00202Q00060006000500122Q000700043Q00202Q0007000700064Q00088Q000700086Q00063Q000200122Q000700023Q00042Q0005001D00012Q00310009000300080006140009001C00013Q00040D3Q001C00012Q00080009000800082Q0006000A6Q0006000B00083Q0004150009001C00010020290003000C00070004280009001A00010004280005001300012Q002B000300023Q00040D3Q00070001002603000200040001000100040D3Q00040001001225000400013Q002603000400260001000200040D3Q00260001001225000200023Q00040D3Q00040001002603000400220001000100040D3Q002200012Q000F00056Q0026000300053Q00122Q000500026Q00065Q00122Q000700023Q00042Q000500340001000E12000200310001000800040D3Q003100012Q003000096Q002E000900014Q00010003000800090004280005002E0001001225000400023Q00040D3Q0022000100040D3Q0004000100040D3Q003E0001002603000200020001000100040D3Q00020001001225000200014Q0020000300033Q001225000200023Q00040D3Q000200012Q00373Q00017Q00", v17(), ...);
