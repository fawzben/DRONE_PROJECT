## Frame structural analysis (simulation on Fusion)

- Based on **the first printable version v1** , we took into account battery weight, thrust force upwards, and gravity on the whole frame. Results :


<img width="1710" height="1107" alt="Screenshot 2026-07-27 at 14 49 58" src="https://github.com/user-attachments/assets/c46fd64a-98e5-47bb-9cdc-0d1836193f31" />


This shows that the arms do not have enough cross section area to resist bending moment, and risk to fail under motor activation. We simply make them longer, bc narrow long is better than wide thin for aerodynamics ig

<img width="1710" height="1107" alt="Screenshot 2026-07-27 at 15 08 37" src="https://github.com/user-attachments/assets/c40732c0-3aab-4f19-82c4-1245d1f8c7be" />


v2 right here. I added 1cm height to the arms, and added load on all four motors


<img width="1382" height="758" alt="Screenshot 2026-08-03 at 15 33 11" src="https://github.com/user-attachments/assets/2a7642c3-62f4-4f81-bea8-b3083677bef6" />
that's the v3 after a few edits. The arms are strong enough, and the top plate was tested with a 50N load, which is way above the actual LiPo battery weight, even with acceleration. This ensures the safety of the drone frame, and we'll print this version
