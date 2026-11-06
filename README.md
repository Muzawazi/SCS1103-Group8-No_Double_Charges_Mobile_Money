Project Title : No Double Charges (Locks and Deadlock prevention in Mobile Money Transfers)

Group Members: 
M.Mazorodze
V.T.Mwakurudza
T.Tanatswa
T.Chihope
M.Mashavera
G.Chifaku
V.Chiwashira
C.Chihuri
M.Chitandara
M.Chamazhika
A.Muningwi
T.Mungure
T.Muzawazi

Question: How much do mutex locks, ordered locking and timeouts reduce double charges and stalled transfers when many mobile-money payments hit the same accounts at once, and at what cost in speed?

Aim: To demonstrate, with a Python transfer demo, how race conditions and deadlocks cause double charges and stalled transfers, and how locking prevents them.

Objectives:
(1) To reproduce a race condition that double-charges an account when payments run without locks;
(2) To reproduce a deadlock between two transfers and show which of the four deadlock conditions each fix removes;
(3) To evaluate each fix by measuring double charges, deadlocks and time per 1000 transfers over 30 runs, and comparing them with the same runs without locks (the baseline); a fix succeeds if it gives zero double charges and zero deadlocks in all 30 runs and takes no more than twice the baseline time.

