## **E7-Bank-Extractor**

An audio .bank extractor for Epic Seven.

This guide will walk you through the process of extracting audio files from .bank files using QuickBMS and FSB_Aud_Extr.

# Prerequisites

Before starting, you'll need the following:

    QuickBMS: A tool for extracting .fsb files from .bank files.

    FSB_Aud_Extr: A tool for extracting audio from .fsb files.

    Epic Seven Game Files: Specifically, the .bank files located in the game’s sound data directory.

# Step 0: Locate the .bank File

The .bank file you're looking for should be found in the following directory:

C:\ProgramData\Smilegate\Games\EpicSeven\data.unpacked\sound\en

    voc.audio_en.bank: This file contains the voice acting audio.

Make a copy of this file and move it to a convenient folder where you’ll be working with it.
Step 1: Extract .bank Files Using QuickBMS

# QuickBMS is a tool that requires user interaction. Follow these steps to extract .fsb files:

    Launch QuickBMS by running quickbms.exe.

    Select the Script: When prompted, choose the dump_fsbs.bms script.

    Choose the .bank File: Select the .bank file you want to extract (e.g., voc.audio_en.bank).

    Select Output Folder: Choose the destination folder where you want the extracted .fsb files to be saved.

    Extraction Process: Wait for QuickBMS to complete the extraction.

After this process, you should have one or more .fsb files in your output folder.
Step 2: Extract Audio from .fsb Files Using FSB_Aud_Extr

Once you've extracted the .fsb files, use FSB_Aud_Extr to extract the audio. You can do this manually via the Command Prompt:
Manual Command Extraction:

    Open Command Prompt (cmd.exe) in the folder where fsb_aud_extr.exe is located.

    Run the following command: fsb_aud_extr.exe <input.fsb>

    Replace <input.fsb> with the name of the .fsb file you want to extract.

The extracted audio will be saved in the same folder where you ran the command.
