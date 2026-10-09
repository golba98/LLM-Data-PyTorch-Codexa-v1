# Retained integration test

`test_general_chat.py.txt` preserves the original `tests/test_general_chat.py` byte for byte. It is an archive, not an active test module. The original requires Training, Architecture and an integration test fixture, so it could not run independently in Data. All three tests remain active in `LLM-From-Scratch/tests/test_general_chat.py`; their ASTs match after import namespace normalization. Data's own twelve component tests remain independently runnable. The text suffix keeps this historical evidence out of pytest collection and distribution packages.
